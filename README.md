# Apache httpd mod_md - Windows MSVC binaries #
- https://github.com/icing/mod_md

----
### Version [2.4.10](https://github.com/icing/mod_md/tree/v2.4.10) 
> 2021-11-24 - commit
>
> 2021-11-24 - build

- **VS17**: toolset 14.30.30818
- **VS16**: toolset 14.29.30133
- **VC15**: toolset 14.16.27023
  - MSVC redist  [x86](https://aka.ms/vs/16/release/vc_redist.x86.exe) - [x64](https://aka.ms/vs/16/release/vc_redist.x64.exe)
- Window Kit: 10.0.22000.0
- **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) releases** __for specified directory__

**Build Scripts** 

- [@nono303/win-build-scripts](https://github.com/nono303/win-build-scripts)
- cflags: `/O2 /GL /MD /Zi`
- ldflags: ` /LTCG /OPT:REF,ICF`

**Build Dependencies**  
*All dependencies are built from sources in the same context*

 - [httpd 2.4.51](https://github.com/apache/httpd/tree/2.4.51) :arrow_right: patched for [openssl 3 PR 258](https://github.com/apache/httpd/pull/258)
 - [jansson 2.14](https://github.com/akheron/jansson/tree/v2.14)

**Runtime Dependencies**

- [openssl 3.0.0](https://github.com/openssl/openssl/tree/openssl-3.0.0) :warning: 

- [curl 7.79.1](https://github.com/curl/curl/tree/curl-7_79_1) :arrow_right: patched for [openssl backend](https://www.apachelounge.com/viewtopic.php?t=8627) - *Thx @**tangent***

