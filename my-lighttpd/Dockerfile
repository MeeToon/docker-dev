FROM alpine:latest
RUN apk add lighttpd
COPY lighttpd.conf /etc/lighttpd/
COPY test.html /var/www/localhost/htdocs/
EXPOSE 8081
CMD /usr/sbin/lighttpd -f /etc/lighttpd/lighttpd.conf && sh
