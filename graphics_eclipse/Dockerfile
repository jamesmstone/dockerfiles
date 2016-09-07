FROM fgrehm/eclipse:v4.4.1
RUN	sudo dpkg --add-architecture i386 && \
		sudo apt-get update && \
		sudo apt-get install -y \
		libxxf86vm1:i386 \
		x11-xserver-utils \
		libglu1-mesa:i386 \
		libglu1-mesa

CMD /usr/local/bin/eclipse
