`./autogen.sh; 
make clean; 
make distclean; 
LD_LIBRARY_PATH="$HOME/demikernel/lib:$HOME/lib/x86_64-linux-gnu" LDFLAGS="-L$HOME/demikernel/lib -L$HOME/lib" CPPFLAGS="-I$HOME/demikernel/include -I$HOME/include" PKG_CONFIG_PATH="$HOME/demikernel/lib/pkgconfig:$HOME/lib/x86_64-linux-gnu/pkgconfig" ./configure --disable-openssl --prefix=$HOME/demikernel; 
LD_LIBRARY_PATH="$HOME/demikernel/lib:$HOME/lib/x86_64-linux-gnu" LDFLAGS="-L$HOME/demikernel/lib -L$HOME/lib" CPPFLAGS="-I$HOME/demikernel/include -I$HOME/include" PKG_CONFIG_PATH="$HOME/demikernel/lib/pkgconfig:$HOME/lib/x86_64-linux-gnu/pkgconfig" make -j20; 
LD_LIBRARY_PATH="$HOME/demikernel/lib:$HOME/lib/x86_64-linux-gnu" LDFLAGS="-L$HOME/demikernel/lib -L$HOME/lib" CPPFLAGS="-I$HOME/demikernel/include -I$HOME/include" PKG_CONFIG_PATH="$HOME/demikernel/lib/pkgconfig:$HOME/lib/x86_64-linux-gnu/pkgconfig" make install
`
