# nginx-fancyindex-bolt-theme

[boltcss](https://github.com/tbolt/boltcss) theme for [nginx fancyindex](https://github.com/aperezdc/ngx-fancyindex)

## preview

![Screenshot 2023-07-27 at 05-32-32 Index of _Example_](https://github.com/pikdum/nginx-fancyindex-bolt-theme/assets/5122800/96238631-b619-4ca2-b456-b394a6316961)


## neat features

* shows fancyindex_footer under header, for showing readmes or similar

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
