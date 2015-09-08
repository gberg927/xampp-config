# xampp-config
wiki for configuring XAMPP

**C:\Windows\System32\drivers\etc\hosts**
_Add_

```
127.0.0.1      	siteName.local
```

**C:\xampp\apache\conf\extra\httpd-vhosts.conf**

_Add_
```
<VirtualHost *>
    DocumentRoot "Path to code"
    ServerName siteName.local
    <Directory "Path to code">
        Require all granted
        AllowOverride All
    </Directory>
</VirtualHost>
```
