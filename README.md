`
./autogen.sh; make clean; make distclean; LD_LIBRARY_PATH="$HOME/demikernel/lib:$HOME/lib/x86_64-linux-gnu" LDFLAGS="-L$HOME/demikernel/lib -L$HOME/lib" CPPFLAGS="-I$HOME/demikernel/include -I$HOME/include" PKG_CONFIG_PATH="$HOME/demikernel/lib/pkgconfig:$HOME/lib/x86_64-linux-gnu/pkgconfig" ./configure --prefix=/usr/local/memcached; LD_LIBRARY_PATH="$HOME/demikernel/lib:$HOME/lib/x86_64-linux-gnu" LDFLAGS="-L$HOME/demikernel/lib -L$HOME/lib" CPPFLAGS="-I$HOME/demikernel/include -I$HOME/include" LD_LIBRARY_PATH="$HOME/demikernel/lib:$HOME/lib/x86_64-linux-gnu" PKG_CONFIG_PATH="$HOME/demikernel/lib/pkgconfig:$HOME/lib/x86_64-linux-gnu/pkgconfig" make -j20
`
`
sudo LD_LIBRARY_PATH=$HOME/demikernel/lib:$HOME/lib/x86_64-linux-gnu:/usr/lib/gcc/x86_64-linux-gnu/9 LIBOS=catnip CONFIG_PATH=$HOME/config.yaml LD_PRELOAD="/usr/lib/gcc/x86_64-linux-gnu/9/libasan.so $HOME/demikernel/lib/libshim.so" ./memcached --threads=8 -l 10.10.1.2 -u root -vvv
`

`
sudo LD_LIBRARY_PATH=$HOME/demikernel/lib:$HOME/lib/x86_64-linux-gnu:/usr/lib/gcc/x86_64-linux-gnu/9 LIBOS=catnip CONFIG_PATH=$HOME/config.yaml LD_PRELOAD="$HOME/demikernel/lib/libshim.so" ./memcached --threads=8 -l 10.10.1.2 -u root -vvv
`
