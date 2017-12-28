FROM alpine:latest
RUN apk --update add git cmake build-base boost cppunit fftw doxygen xmlto python py-pip swig py-numpy && \
pip install six mako

RUN git clone --recursive git://git.gnuradio.org/gnuradio /gnuradio
#ADD http://gnuradio.org/releases/gnuradio/gnuradio-3.7.10.1.tar.gz /gnuradio.tar.gz

RUN cd gnuradio && \
mkdir build  && \
cd build && \
cmake /gnuradio # && \
make  && \
make test && \
make install

ENTRYPOINT ["gnuradio-companion"]
