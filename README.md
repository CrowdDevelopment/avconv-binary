Source code: https://libav.org/releases/libav-9.17.tar.gz

Compilation:

    tar -xvf libav-9.17.tar.gz
    cd libav-9.17
    ./configure --enable-static --enable-libmp3lame --enable-runtime-cpudetect \
      --disable-doc --disable-avdevice --disable-w32threads --disable-network \
      --disable-debug --disable-devices --disable-indevs --disable-encoders \
      --enable-encoder=libmp3lame --disable-decoders --enable-decoder=amrnb \
      --enable-decoder=amrwb
    make

Make sure to run 'make distclean' if u want to repeat compilation instructions.

avconv binary will be created and placed in root directory.

libmp3lame can be taken directly from ubuntu 14.04 at path "/usr/lib/x86_64-linux-gnu/libmp3lame.so". 
Package "libmp3lame-dev".
