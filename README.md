# Apache httpd mod_md - Windows MSVC binaries #
- https://github.com/icing/mod_md
- https://httpd.apache.org/docs/trunk/mod/mod_md.html

----
## Version [1.1.19](https://github.com/icing/mod_md/tree/v1.1.19)** a.k.a 1.99.8-git + mod_ssl [patched](https://github.com/icing/mod_md/blob/master/patches/mod_ssl_md2-2.4.x.diff) from httpd tag [2.4.39](https://github.com/apache/httpd/tree/2.4.39)   
> 
> 2019-03-22   **VC15**
- MSVC 15.9.9 / 19.16.27027.1
- Window Kit 10.0.17763.0
>
> 2019-05-07 **VS16**
- MSVC 16.1.0 preview 3.0 / 14.21.27619.1
- Window Kit 10.0.18362.0  
>
>
- **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) releases** __for specified directory__
- MSVC redist 14.21.27619 [x86](https://download.visualstudio.microsoft.com/download/pr/1a6314bb-c949-42e9-925f-1c0bf4eb00de/41482628dd05373a7c24b0d43ae1753e/vc_redist.x86.exe) - [x64](https://download.visualstudio.microsoft.com/download/pr/0eac0881-2173-4d79-bee7-fda4dccb0005/aa1dfcd3b6c304fa8b8b57d1e3d6ae63/vc_redist.x64.exe)

**Build Dependencies**  
*All dependencies are built from sources in the same context*
 - [openssl 1.1.1b](https://github.com/openssl/openssl/tree/OpenSSL_1_1_1b) - __crypto header [patched](https://github.com/openssl/openssl/commit/ef45aa14c5af024fcb8bef1c9007f3d1c115bd85) for [#2865](https://github.com/openssl/openssl/issues/2865)__
 - [curl 7.64.0](https://github.com/curl/curl/tree/curl-7_64_0)  
 - [jansson 2.12](https://github.com/akheron/jansson/tree/v2.12)
