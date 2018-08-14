FROM haskell:8.4.3
MAINTAINER Scott Fleischman <scott-fleischman@users.noreply.github.com>
RUN stack --resolver lts-12.6 install Agda && \
  find /root/.stack -type f -not -wholename '*Agda*' -delete && \
  find /root/.stack -type d -empty -delete
CMD agda
