# apache httpd mod_md windows builds #

----
- https://github.com/icing/mod_md
- https://httpd.apache.org/docs/trunk/mod/mod_md.html  

----
2019-02-07
**v1.99.7-git + mod_ssl [patched](https://github.com/icing/mod_md/blob/master/patches/mod_ssl_md2-2.4.x.diff) from httpd tag 2.4.38**   

- **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) build** __only on specified directory__
- MSVC 15.9.6 / 19.16.27026.1
  - MSVC redist 14.16.27024 [x86](https://aka.ms/vs/15/release/VC_redist.x86.exe) - [x64](https://aka.ms/vs/15/release/VC_redist.x64.exe)
- Window Kit 10.0.17763.0
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
> - [Openssl 1.1.1a ](https://github.com/openssl/openssl/tree/OpenSSL_1_1_1a)  
> - [curl 7.64.0](https://github.com/curl/curl/tree/curl-7_64_0)  
> - [jansson 2.12 ](https://github.com/akheron/jansson/tree/v2.12)