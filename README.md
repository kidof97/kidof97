pkg upgrade -y
Run pkg install git cmake libuv clang nano -y
Run git clone --single-branch https://github.com/turtlecoin/ninjarig
Run cd ninjarig
Run mkdir build && cd build
Run cmake .. -DWITH_HTTPD=OFF -DWITH_TLS=OFF -DWITH_OPENCL=OFF -DWITH_CUDA=OFF -DCMAKE_BUILD_TYPE=Release
Run make -j2
Run cp ../src/config.json config.json
Run nano config.json and adjust your config settings to match you wallet and pool etc.
Configure it
Run ./ninjarig-notls
