FROM walm/ruby:0.1.0
MAINTAINER Andreas Wålm "andreas@walm.net"

RUN bash -c ' \
  apt-get update -qq ;\
  apt-get install -q -y software-properties-common ;\
  \
  echo "# Installing Node.js" ;\
  add-apt-repository -y ppa:chris-lea/node.js ;\
  apt-get -q -y install nodejs ;\
  \
  echo "# Cleaning up" ;\
  apt-get remove -qq -y software-properties-common ;\
  apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /setup /build ;\
  true'
# END RUN
