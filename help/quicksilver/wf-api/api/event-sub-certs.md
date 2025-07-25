---
content-type: api
navigation-topic: api-navigation-topic
title: 事件订阅证书
description: 事件订阅证书
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: 2c5a4ff65088652b67099d187e6ee4c11d80a3b3
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---

# 为事件订阅配置客户端TLS

<!--Configuring Client TLS for Event Subscription
Steps to Verify Workfront's Client Certificate
Examples for Server configuration
NGINX
Apache
Certificate to Environment Mapping
Certificates
Production
Preview
Sandbox 1
Sandbox 2
-->

通过客户端TLS，可验证您收到的事件订阅消息是否实际来自Adobe Workfront。 要启用此功能，必须将您的服务器配置为请求和验证Workfront的x509证书。


>[!NOTE]
>
>如果事件订阅将事件发送到到的服务器支持版本1.3，则事件订阅使用TLS版本1.3。如果连接服务器不支持版本1.3，则事件订阅使用TLS版本1.2。



## 验证Workfront的客户端证书

此过程假定您的服务器配置为接受TLS连接。 Workfront不支持自签名证书。

通常，为服务器启用客户端身份验证所需的步骤如下：

1. 下载DigiCert全局根CA证书的PEM版本。
1. 打开客户端证书验证。

   将步骤1中的CA证书指定为可信证书。

1. 将验证深度设置为2，因为我们的证书实际由DigiCert SHA2安全服务器CA签名，该CA是DigiCert全局根CA下的中间CA。
1. 通过检查客户端证书的主题域名，验证其是否确实来自Workfront。

## 服务器配置示例

### 恩金克斯

```
server {

    listen 443 ssl default_server;
    # ... existing SSL configuration for server authentication ...

    ssl_verify_client on;
    ssl_client_certificate /path/to/DigiCert_Global_Root_CA.pem;
    ssl_verify_depth 2;

        # ... existing location configuration ...
    }
}
```

有关详细信息，请参阅[NGiNX文档ngx_http_ssl_module](https://nginx.org/en/docs/http/ngx_http_ssl_module.html)。

### Apache

```
Listen 443
<VirtualHost *:443>
    # ... existing SSL configuration for server authentication ...

    SSLVerifyClient require
    SSLCACertificateFile "/path/to/DigiCert_Global_Root_CA.pem"
    SSLVerifyDepth 2
</VirtualHost>

<Directory /var/www/>
    Require expr "%{SSL_CLIENT_S_DN_CN} == <>"

    # ... existing directory configuration ...
</Directory>
```

有关更多信息，请参阅

* [客户端身份验证和访问控制](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Apache模块mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## 证书到环境的映射

| WF环境 | 证书公用名 | 证书主题(DN) |
| -- | -- | -- |
| 生产 | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront， Inc./CN=*.prod.eventsubscriptions.workfront.com |
| 预览 | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront， Inc./CN=*.preview.eventsubscriptions.workfront.com |
| Sandbox 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront， Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| Sandbox 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront， Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## 下载证书

单击以下链接以下载客户端证书。

* [客户端证书 — 生产环境](assets/prod-environment-nov-2024.crt)
* [客户端证书 — 预览环境](assets/preview-environment-nov-2024.crt)
* [客户端证书 — 沙盒环境](assets/sandbox-environment-nov-2024.crt)

>[!NOTE]
>
>您可以对两个沙盒环境使用相同的客户端证书。
