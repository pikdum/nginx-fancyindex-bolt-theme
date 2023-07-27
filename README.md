# nginx-fancyindex-bolt-theme

[boltcss](https://github.com/tbolt/boltcss) theme for [nginx fancyindex](https://github.com/aperezdc/ngx-fancyindex)

## neat features

* shows README.txt content under header

## example config

```
server {
    listen 80;
    server_name default_server;

    root /storage/;

    location / {
        fancyindex on;
        fancyindex_exact_size off;
        fancyindex_localtime on;
        fancyindex_css_href 'https://cdn.jsdelivr.net/gh/pikdum/nginx-fancyindex-bolt-theme/fancyindex-bolt.css';
        fancyindex_footer README.txt;
    }
}
```
