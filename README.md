# Apache httpd mod_md - Windows MSVC binaries #
- https://github.com/icing/mod_md
- https://httpd.apache.org/docs/trunk/mod/mod_md.html

----
## Version [1.99.11](https://github.com/icing/mod_md/tree/v1.99.11) + mod_ssl [patched](https://github.com/icing/mod_md/blob/master/patches/mod_ssl_md2-2.4.x.diff) from httpd tag [2.4.39](https://github.com/apache/httpd/tree/2.4.39)   
> 
> 2019-05-16 **VS16**
- MSVC 16.1.0 preview 3.0 / 14.21.27619.1
- Window Kit 10.0.18362.0  
----
- **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) releases** __for specified directory__
- MSVC redist 14.21.27619 [x86](https://download.visualstudio.microsoft.com/download/pr/59e7fad0-c074-49e8-a815-77cb7083f910/9d4c6916d07433832c836646e65e81df/vc_redist.x86.exe) - [x64](https://download.visualstudio.microsoft.com/download/pr/b28932f6-8d79-46f1-8385-e0a8bdf3c1e0/1adf822fa2d810d2c736bf97efe84e34/vc_redist.x64.exe)

**Build Dependencies**  
*All dependencies are built from sources in the same context*
 - [openssl 1.1.1b](https://github.com/openssl/openssl/tree/OpenSSL_1_1_1b) - __crypto header [patched](https://github.com/openssl/openssl/commit/ef45aa14c5af024fcb8bef1c9007f3d1c115bd85) for [#2865](https://github.com/openssl/openssl/issues/2865)__
 - [curl 7.64.1](https://github.com/curl/curl/tree/curl-7_64_1)  
 - [jansson 2.12](https://github.com/akheron/jansson/tree/v2.12)
