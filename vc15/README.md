If you want to build it from [httpd branch 2.4.x-mod_md](https://github.com/apache/httpd/tree/2.4.x-mod_md)  

1) deps
> - [Openssl 1.1.0g ](https://github.com/openssl/openssl/tree/OpenSSL_1_1_0g)  
> - [curl 7.58](https://github.com/curl/curl)  
> - [jansson 2.10](https://github.com/akheron/jansson)  

2) Apply [CMakeLists.txt.patch](https://github.com/nono303/mod_md/blob/master/vc15/CMakeLists.txt.patch) on src `/CMakeLists.txt`

3) Add `-DJANSSON_INCLUDE_DIR=/install/include` and `-DJANSSON_LIBRARIES=/install/lib/jansson.lib` to your cmake command line

This is it!