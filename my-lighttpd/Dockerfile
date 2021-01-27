FROM alpine:latest
RUN apk add lighttpd
COPY lighttpd.conf /etc/lighttpd/
COPY test.html /var/www/localhost/htdocs/
EXPOSE 8081

#---v0.0
#CMD /usr/sbin/lighttpd -f /etc/lighttpd/lighttpd.conf
#---v0.1
#CMD ["/usr/sbin/lighttpd", "-f", "/etc/lighttpd/lighttpd.conf"]

#---v1.0
#CMD /usr/sbin/lighttpd -f /etc/lighttpd/lighttpd.conf && sh
#---v1.1
#CMD ["/usr/sbin/lighttpd", "-f", "/etc/lighttpd/lighttpd.conf", "&&", "sh"]
#---v1.2
#CMD ["sh", "/usr/sbin/lighttpd -f /etc/lighttpd/lighttpd.conf && sleep 3600"]

#---v2.0
#CMD /usr/sbin/lighttpd -f /etc/lighttpd/lighttpd.conf -D          

#---v3.0 end with "sh"
#---v3.1 end with "sleep"
#COPY app.sh /
#ENTRYPOINT ["sh", "/app.sh"]
