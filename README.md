# Apache httpd mod_md - Windows MSVC binaries #
- https://github.com/icing/mod_md

----
## `VC15 & VS16`
- VS16 : toolset 14.28.29333
- VC15 : toolset 14.16.27023
  - MSVC redist  [x86](https://aka.ms/vs/16/release/vc_redist.x86.exe) - [x64](https://aka.ms/vs/16/release/vc_redist.x64.exe)
- Window Kit 10.0.19041.0
- **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) releases** __for specified directory__

### Version [2.3.7](https://github.com/icing/mod_md/tree/v2.3.7)
> 2021-02-05

**Build Scripts** 

- [@nono303/win-build-scripts](https://github.com/nono303/win-build-scripts)
- cflags: `/O2 /GL /MD /Zi`
- ldflags: `/LTCG /OPT:ICF`

**Build Dependencies**  
*All dependencies are built from sources in the same context*

 - [curl 7.75.0](https://github.com/curl/curl/tree/curl-7_75_0)  
 - [httpd 2.4.46](https://github.com/apache/httpd/tree/2.4.46)   
 - [jansson 2.13.1](https://github.com/akheron/jansson/tree/v2.13.1)
 - [openssl 1.1.1i](https://github.com/openssl/openssl/tree/OpenSSL_1_1_1i)
