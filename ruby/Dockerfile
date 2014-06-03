FROM walm/ruby:0.1.0
MAINTAINER Andreas Wålm "andreas@walm.net"

RUN bash -c '\
  apt-get update -qq ;\
  \
  echo "# Installing Node.js" ;\
  apt-get -q -y install nodejs npm ;\
  ln -s /usr/bin/nodejs /usr/bin/node ;\
  \
  echo "# Cleaning up" ;\
  apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /setup /build ;\
'
# END RUN
