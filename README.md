# Apache httpd mod_md - Windows MSVC binaries #
- https://github.com/icing/mod_md
- https://httpd.apache.org/docs/trunk/mod/mod_md.html

----
2019-02-27  
> **version [1.99.7-git](https://github.com/icing/mod_md/tree/v1.99.7) + mod_ssl [patched](https://github.com/icing/mod_md/blob/master/patches/mod_ssl_md2-2.4.x.diff) from httpd tag [2.4.38](https://github.com/apache/httpd/tree/2.4.38)**   

- MSVC 15.9.7 / 19.16.27027.1
  - MSVC redist 14.16.27024.1 [x86](https://aka.ms/vs/15/release/VC_redist.x86.exe) - [x64](https://aka.ms/vs/15/release/VC_redist.x64.exe)
- Window Kit 10.0.17763.0
- **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) releases** __for specified directory__

**Build Dependencies**  
*All dependencies are built from sources in the same context*
 - [openssl 1.1.1b](https://github.com/openssl/openssl/tree/OpenSSL_1_1_1b) - __crypto header [patched](https://github.com/openssl/openssl/commit/ef45aa14c5af024fcb8bef1c9007f3d1c115bd85) for [#2865](https://github.com/openssl/openssl/issues/2865)__
 - [curl 7.64.0](https://github.com/curl/curl/tree/curl-7_64_0)  
 - [jansson 2.12](https://github.com/akheron/jansson/tree/v2.12)
----
```
mod_md.so               /x64/               x64 ltcg
mod_ssl.so              /x64/               x64 ltcg
mod_md.so               /x64-avx/           x64 ltcg avx (86)
mod_ssl.so              /x64-avx/           x64 ltcg avx (15)
mod_md.so               /x86/               x86 ltcg
mod_ssl.so              /x86/               x86 ltcg
mod_md.so               /x86-avx/           x86 ltcg avx (125)
mod_ssl.so              /x86-avx/           x86 ltcg avx (34)
```  