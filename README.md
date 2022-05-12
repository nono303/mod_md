# Apache httpd mod_md - Windows MSVC binaries #
- https://github.com/icing/mod_md

----
### Version [2.4.16](https://github.com/icing/mod_md/tree/v2.4.16) 
> 2022-05-11 - commit
>
> 2022-05-12 - build

- **VS17** toolset: 14.33.31424
- **VS16** toolset: 14.29.30133
- **VC15** toolset: 14.16.27023
- MSVC redist:  [x86](https://aka.ms/vs/16/release/vc_redist.x86.exe) - [x64](https://aka.ms/vs/16/release/vc_redist.x64.exe)
- Window Kit: 10.0.22000.0
- **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) releases** _in specified directory_

**Build Scripts** 

- [@nono303/win-build-scripts](https://github.com/nono303/win-build-scripts)
- cflags: `/O2 /GL /MD /Zi`
- ldflags: ` /LTCG /OPT:REF,ICF`

**Build Dependencies**  
*All dependencies are built from sources in the same context*

 - [httpd 2.4.53](https://github.com/apache/httpd/tree/2.4.53)
 - [jansson 2.14](https://github.com/akheron/jansson/tree/v2.14)

**Runtime Dependencies**

- [openssl 3.0.3](https://github.com/openssl/openssl/tree/openssl-3.0.3) :warning: 
- [curl 7.83.1](https://github.com/curl/curl/tree/curl-7_83_1) :arrow_right: patched for [openssl backend](https://www.apachelounge.com/viewtopic.php?t=8627) - *Thx @**tangent***

