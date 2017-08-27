# Nginx Docker Image

[Busybox](https://www.busybox.net)-based, [UPX](https://upx.github.io)-compressed images for nginx v1.13.4.

### Branches / Images

#### Dockerfile.source

[![](https://images.microbadger.com/badges/version/nevstokes/nginx:src.svg)](https://microbadger.com/images/nevstokes/nginx:src "Get your own version badge on microbadger.com") [![](https://images.microbadger.com/badges/image/nevstokes/nginx:src.svg)](https://microbadger.com/images/nevstokes/nginx:src "Get your own image badge on microbadger.com") [![](https://images.microbadger.com/badges/commit/nevstokes/nginx.svg)](https://microbadger.com/images/nevstokes/nginx "Get your own commit badge on microbadger.com")

GnuPG verified nginx source code for building the other images in this repository.

#### Dockerfile

[![](https://images.microbadger.com/badges/version/nevstokes/nginx.svg)](https://microbadger.com/images/nevstokes/nginx "Get your own version badge on microbadger.com") [![](https://images.microbadger.com/badges/image/nevstokes/nginx.svg)](https://microbadger.com/images/nevstokes/nginx "Get your own image badge on microbadger.com") [![](https://images.microbadger.com/badges/commit/nevstokes/nginx.svg)](https://microbadger.com/images/nevstokes/nginx "Get your own commit badge on microbadger.com")

Small vanilla build of nginx, without many of the less frequently used modules compiled (e.g. media pseudo-streaming, image filters, mail, DAV, etc).

#### Dockerfile.custom

[![](https://images.microbadger.com/badges/version/nevstokes/nginx:custom.svg)](https://microbadger.com/images/nevstokes/nginx:custom "Get your own version badge on microbadger.com") [![](https://images.microbadger.com/badges/image/nevstokes/nginx:custom.svg)](https://microbadger.com/images/nevstokes/nginx:custom "Get your own image badge on microbadger.com") [![](https://images.microbadger.com/badges/commit/nevstokes/nginx:custom.svg)](https://microbadger.com/images/nevstokes/nginx:custom "Get your own commit badge on microbadger.com")

As per the vanilla build but with [Brotli](https://github.com/google/ngx_brotli) compression, [Headers More](https://github.com/openresty/headers-more-nginx-module) and [Cache Purge](https://github.com/FRiCKLE/ngx_cache_purge) modules compiled.

Available from [Docker Hub](https://hub.docker.com/r/nevstokes/nginx/) with:

    $ docker pull nevstokes/nginx[:latest]
    $ docker pull nevstokes/nginx:custom
    $ docker pull nevstokes/nginx:src

#### Caveat lector
This is the result of general tinkering and experimentation. Hopefully it will be something at least of interest to someone but it's likely unwise to be using this for anything critically important.
