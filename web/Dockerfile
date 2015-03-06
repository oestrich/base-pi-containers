FROM oestrich/base-pi
MAINTAINER Eric Oestrich <eric@oestrich.org>

RUN pacman -Syu --noconfirm \
  && pacman -S --noconfirm \
    libxml2 \
    libxslt \
    imagemagick \
    openssl \
    postgresql \
    python2 \
    nodejs \
    glusterfs \
  && pacman -Sc --noconfirm

RUN gem install bundler
RUN gem install foreman
RUN gem install nokogiri --version 1.6.5
