FROM oestrich/arch-pi
MAINTAINER Eric Oestrich <eric@oestrich.org>

RUN pacman -Syu --noconfirm
RUN pacman -S --noconfirm \
	    base-devel \
	    libffi \
	    libyaml \
	    openssl \
	    zlib \
	    git

RUN git clone https://github.com/sstephenson/ruby-build.git
RUN cd ruby-build && ./install.sh
RUN ruby-build 2.2.0 /opt/ruby
ENV PATH $PATH:/opt/ruby/bin
