# redirect-http-to-https-htaccess

- copas ke htaccess domain

<code>RewriteEngine On</code> <br>
<code>RewriteCond %{HTTPS} off</code> <br>
<code>RewriteRule ^(.*)$ https://%{HTTP_HOST}%{REQUEST_URI} [L,R=301]</code>
