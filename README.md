# Apache httpd mod_md - Windows MSVC binaries #
- https://github.com/icing/mod_md
- https://httpd.apache.org/docs/trunk/mod/mod_md.html

----
## Version [2.0.7](https://github.com/icing/mod_md/tree/v2.0.7) + mod_ssl [patched](https://github.com/icing/mod_md/blob/master/patches/mod_ssl_md2-2.4.x.diff) from httpd tag [2.4.39](https://github.com/apache/httpd/tree/2.4.39)   
> 
> 2019-07-10
- Visual Studio 2019 v16.1.3
- VS16 : toolset 14.21.27702
- VC15 : toolset 14.16.27023
- Window Kit 10.0.18362.0  
----
- **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) releases** __for specified directory__
- MSVC redist (https://gitlab.com/stdout12/adns/tags)

**Build Dependencies**  
*All dependencies are built from sources in the same context*
 - [openssl 1.1.1c](https://github.com/openssl/openssl/tree/OpenSSL_1_1_1c)
 - [curl 7.65.1](https://github.com/curl/curl/tree/curl-7_65_1)  
 - [jansson 2.12](https://github.com/akheron/jansson/tree/v2.12)
