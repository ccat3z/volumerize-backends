FROM blacklabelops/volumerize:latest

RUN echo $(sed -n "1p" /etc/apk/repositories | sed "s/v[^\/]*\/[^\/]*$/edge\/main/") >> /etc/apk/repositories && \
    echo $(sed -n "1p" /etc/apk/repositories | sed "s/v[^\/]*\/[^\/]*$/edge\/testing/") >> /etc/apk/repositories

RUN apk --no-cache add megatools
