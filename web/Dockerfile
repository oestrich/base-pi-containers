FROM oestrich/base-pi
MAINTAINER Eric Oestrich <eric@oestrich.org>

RUN pacman -Syu --noconfirm
RUN pacman -S --noconfirm \
      libxml2 \
      libxslt \
      imagemagick \
      openssl \
      postgresql \
      python2

RUN gem install bundler
RUN gem install foreman
RUN gem install libv8 --version 3.16.14.7
RUN gem install nokogiri --version 1.6.5
