# Apache httpd mod_md - Windows MSVC binaries #
- https://github.com/icing/mod_md

----
### Version [2.4.5](https://github.com/icing/mod_md/tree/v2.4.5)
> 2021-09-01 - commit
>
> 2021-09-29 - build

- **VS17**: toolset 14.30.30528
- **VS16**: toolset 14.29.30132
- **VC15**: toolset 14.16.27023
  - MSVC redist  [x86](https://aka.ms/vs/16/release/vc_redist.x86.exe) - [x64](https://aka.ms/vs/16/release/vc_redist.x64.exe)
- Window Kit: 10.0.20348.0
- **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) releases** __for specified directory__

**Build Scripts** 

- [@nono303/win-build-scripts](https://github.com/nono303/win-build-scripts)
- cflags: `/O2 /GL /MD /Zi`
- ldflags: ` /LTCG /OPT:REF,ICF`

**Build Dependencies**  
*All dependencies are built from sources in the same context*

 - [httpd 2.4.49](https://github.com/apache/httpd/tree/2.4.49)   
 - [jansson 2.14](https://github.com/akheron/jansson/tree/v2.14)
 - [openssl 1.1.1l](https://github.com/openssl/openssl/tree/OpenSSL_1_1_1l)

**Runtime Dependencies**

- [curl 7.79.1](https://github.com/curl/curl/tree/curl-7_79_1) :arrow_right: [patched](https://www.apachelounge.com/viewtopic.php?t=8627) for openssl backend - *Thx @**tangent***
