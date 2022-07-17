# Apache httpd mod_md - Windows MSVC binaries #
- https://github.com/icing/mod_md

----
### Version [2.4.18](https://github.com/icing/mod_md/tree/v2.4.18) 
> 2022-07-15 - commit
>
> 2022-07-17 - build

- **VS17** toolset: 14.33.31627
- **VS16** toolset: 14.29.30133
- **VC15** toolset: 14.16.27023
- MSVC redist:  [x86](https://aka.ms/vs/16/release/vc_redist.x86.exe) - [x64](https://aka.ms/vs/16/release/vc_redist.x64.exe)
- Window Kit: 10.0.22000.0
- **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) releases** _in specified directory_

**Build Scripts** 

- [@nono303/win-build-scripts](https://github.com/nono303/win-build-scripts)
- cflags: `/O2 /GL /MD /Zi`
- ldflags: ` /LTCG /OPT:REF,ICF`

**Build  & Runtime Dependencies**

> * All dependencies are built from sources in the same context
>
> * Check it with`dumpbin /DEPENDENTS mod_md.so`

- [curl 7.84.0](https://github.com/curl/curl/tree/curl-7_83_1) - `libcurl.dll` 
  - build with schannel & openssl TLS backend _(see [CURL_SSL_BACKEND](https://cran.r-project.org/web/packages/curl/vignettes/windows.html))_
  - :arrow_right: patched for [openssl TLS backend](https://www.apachelounge.com/viewtopic.php?t=8627) using Windows `native_ca_store` - *Thx @**tangent***

- :warning:[openssl 3.0.5](https://github.com/openssl/openssl/tree/openssl-3.0.5) - `libcrypto-3-x64.dll` || `libcrypto-3.dll` 
- [apr 1.8.0-dev](https://github.com/apache/apr) - `libapr-1.dll`
- [apr-util 1.7.0-dev](https://github.com/apache/apr-util) - `libaprutil-1.dll`
- [jansson 2.14](https://github.com/akheron/jansson/tree/v2.14) - `jansson.dll`
- [httpd 2.4.54](https://github.com/apache/httpd/tree/2.4.54) - `libhttpd.dll`
