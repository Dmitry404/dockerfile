# Oracle JRE 8u121-b13
FROM dmitry404/ubuntu-base
MAINTAINER dmity404@gmail.com

RUN wget --no-check-certificate --no-cookies --header "Cookie: oraclelicense=accept-securebackup-cookie" \
		 http://download.oracle.com/otn-pub/java/jdk/8u121-b13/e9e7ea248e2c4826b92b3f075a80e441/jre-8u121-linux-x64.tar.gz \
		 && tar xzf jre-8u121-linux-x64.tar.gz \
	 	 && rm -f jre-8u121-linux-x64.tar.gz

RUN mkdir -p /usr/lib/jvm/java-8-oracle \
		 && mv jre1.8.0_121 /usr/lib/jvm/java-8-oracle/jre \
		 && chown root:root -R /usr/lib/jvm/java-8-oracle/jre \
		 && update-alternatives --install /usr/bin/java java /usr/lib/jvm/java-8-oracle/jre/bin/java 1 \
		 && update-alternatives --set java  /usr/lib/jvm/java-8-oracle/jre/bin/java

CMD ["java", "-version"]
