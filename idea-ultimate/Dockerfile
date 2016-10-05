FROM	openjdk:8-jdk
MAINTAINER	James Stone
ADD 	https://download.jetbrains.com/idea/ideaIU-2016.2.4.tar.gz /tmp/intellij.tar.gz
RUN		mkdir -p /config \
			&& mkdir -p /opt/intellij \
			&& tar -xf /tmp/intellij.tar.gz --strip-components=1 -C /opt/intellij \
			&& rm /tmp/intellij.tar.gz
COPY	./idea.properties /opt/intellij/bin/idea.properties
COPY	./idea /usr/local/bin/idea
ENTRYPOINT	["/usr/local/bin/idea"]
