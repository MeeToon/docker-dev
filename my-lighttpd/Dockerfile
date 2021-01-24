FROM alpine:latest
RUN apk add lighttpd
COPY lighttpd.conf /etc/lighttpd/
COPY test.html /var/www/localhost/htdocs/
EXPOSE 8081
#---v1.0
#CMD /usr/sbin/lighttpd -f /etc/lighttpd/lighttpd.conf && sh
#---v2.0
#CMD /usr/sbin/lighttpd -f /etc/lighttpd/lighttpd.conf -D          
#---v3.0
COPY app.sh /
ENTRYPOINT ["sh", "/app.sh"]
