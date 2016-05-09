FROM java:7-jre

MAINTAINER jorgechavez77

ADD http://docker.server.com/mule-standalone-3.4.0.tar.gz /opt/

RUN cd /opt && tar xvzf  mule-standalone-3.4.0.tar.gz && rm mule-standalone-3.4.0.tar.gz && ln -s /opt/mule-standalone-3.4.0 /opt/mule

ENV MULE_HOME /opt/mule

VOLUME ["/opt/mule/logs", "/opt/mule/conf", "/opt/mule/apps", "/opt/mule/domains"]

WORKDIR /opt/mule

CMD [ "/opt/mule/bin/mule" ]

EXPOSE 8081

