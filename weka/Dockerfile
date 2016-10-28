	
	
	
FROM	java:latest
ADD	http://www.cs.waikato.ac.nz/~ml/weka/snapshots/stable-3-8.zip	./weka.zip
RUN	unzip ./weka.zip \
	&& rm ./weka.zip
CMD	["java","-jar","/weka/weka.jar"]
