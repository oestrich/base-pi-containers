FROM oestrich/arch-pi
MAINTAINER Eric Oestrich "eric@oestrich.org"

RUN pacman -Syu --noconfirm \
  && pacman -S --noconfirm \
    nginx \
  && pacman -Sc --noconfirm

RUN ln -sf /dev/stdout /var/log/nginx/access.log
RUN ln -sf /dev/stderr /var/log/nginx/error.log

VOLUME ["/var/cache/nginx"]

EXPOSE 80 443

CMD ["nginx", "-g", "daemon off;"]
