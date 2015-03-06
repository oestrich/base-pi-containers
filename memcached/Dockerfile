FROM oestrich/arch-pi
MAINTAINER Eric Oestrich "eric@oestrich.org"

RUN pacman -Syu --noconfirm \
  && pacman -S --noconfirm \
    memcached \
  && pacman -Sc --noconfirm

EXPOSE 11211

CMD ["memcached", "-v", "-m", "64", "-p", "11211", "-u", "nobody"]
