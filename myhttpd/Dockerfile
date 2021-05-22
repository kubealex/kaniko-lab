FROM alpine
LABEL description="Creating a custom httpd image"
MAINTAINER Alessandro Rossi <al.rossi87@gmail.com>
RUN apt-get install -y httpd
EXPOSE 80
ENV TestVar "This is a test environment variable"
ADD index.html /var/www/html/
#COPY ./src/ /var/www/html/
USER root
ENTRYPOINT ["/usr/sbin/httpd"]
CMD ["-D", "FOREGROUND"]
