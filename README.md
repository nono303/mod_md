# Apache httpd mod_md - Windows MSVC binaries #
- https://github.com/icing/mod_md

----
### Version [2.4.26](https://github.com/icing/mod_md/tree/v2.4.26) 
> 2024-01-03 - commit
>
> 2024-01-04 - build

- **VS17** toolset: 14.39.33321
- **VS16** toolset: 14.29.30133
- **VC15** toolset: 14.16.27023
- MSVC redist:  [x86](https://aka.ms/vs/16/release/vc_redist.x86.exe) - [x64](https://aka.ms/vs/16/release/vc_redist.x64.exe)
- Window Kit: 10.0.22621.0
- **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) releases** _in specified directory_

[**How to get the good version**](https://github.com/nono303/PHP-memcache-dll#how-to-get-the-good-version)

**Build Scripts** 

- [@nono303/win-build-scripts](https://github.com/nono303/win-build-scripts)
- cflags: `/O2 /GL /MD /Zi`
- ldflags: ` /LTCG /OPT:REF,ICF`

**Build  & Runtime Dependencies**

> * All dependencies are built from sources in the same context
>
> * Check it with `dumpbin /DEPENDENTS mod_md.so`

- [curl 8.5.0](https://github.com/curl/curl/tree/curl-8_5_0) - `libcurl.dll` 
  - **MultiSSL** build with OpenSSL & Schannel _(see [CURL_SSL_BACKEND](https://cran.r-project.org/web/packages/curl/vignettes/windows.html))_
  - :arrow_right: patched for [OpenSSL backend](https://www.apachelounge.com/viewtopic.php?t=8627) using Windows `native_ca_store` - *Thx @**tangent***

- [openssl 3.1.4](https://github.com/openssl/openssl/tree/openssl-3.1.4) - `libcrypto-3-x64.dll` || `libcrypto-3.dll` 
- [apr 1.8.0-dev](https://github.com/apache/apr) - `libapr-1.dll`
- [apr-util 1.7.0-dev](https://github.com/apache/apr-util) - `libaprutil-1.dll`
- [jansson 2.14](https://github.com/akheron/jansson/tree/v2.14) - `jansson.dll`
- [httpd 2.4.58](https://github.com/apache/httpd/tree/2.4.58) - `libhttpd.dll`
