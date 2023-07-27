# nginx-fancyindex-bolt-theme

[boltcss](https://github.com/tbolt/boltcss) theme for [nginx fancyindex](https://github.com/aperezdc/ngx-fancyindex)

## preview

![image](https://github.com/pikdum/nginx-fancyindex-bolt-theme/assets/5122800/df482675-6bbd-4051-ad18-5a25cb3cdafd)


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
