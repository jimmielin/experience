# Lighttpd with Laravel 5

```
$HTTP["host"] =~ "(^|\.)example\.com$" {
    server.document-root = "/var/www/public"

    alias.url = ()
    url.redirect = ()
    url.rewrite-if-not-file = (
                "^/(css|img|js|fonts)/.*\.(jpg|jpeg|gif|png|swf|avi|mpg|mpeg|mp3|flv|ico|css|js|woff|ttf)$" => "$0",
                "^/(favicon\.ico|robots\.txt|sitemap\.xml)$" => "$0",
                "^/[^\?]*(\?.*)?$" => "index.php/$1"
    )
}
```