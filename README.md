# apache httpd mod_md windows builds #

----
- https://github.com/icing/mod_md
- https://httpd.apache.org/docs/trunk/mod/mod_md.html  

----
**v1.99.0-git + mod_ssl [patched](https://github.com/icing/mod_md/blob/master/patches/mod_ssl_md2-2.4.x.diff) from httpd 2.4.38**  

2019-01-21
 - pdb for so & dll
 - janson build dep 
 - curl build dep compiled with Winssl to avoid issue [#14](https://github.com/icing/mod_md/issues/14)  
    ```Enabled features: WinSSL libz AsynchDNS SSPI SPNEGO Kerberos NTLM```  
    ```Enabled protocols: DICT FILE FTP FTPS GOPHER HTTP HTTPS IMAP IMAPS LDAP POP3 POP3S RTSP SMTP SMTPS TELNET TFTP```

> - MSVC 15.9.5 / 19.16.27026.1
>   - MSVC15 redist 14.16.27024 [x86](https://aka.ms/vs/15/release/VC_redist.x86.exe) - [x64](https://aka.ms/vs/15/release/VC_redist.x64.exe)
> - Window Kit 10.0.17763.0
> - **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) build** __only on specified directoy__
    
> - [Openssl 1.1.1a ](https://github.com/openssl/openssl/tree/OpenSSL_1_1_1a)  
> - [curl 7.63.0](https://github.com/curl/curl/tree/curl-7_63_0)  
> - [jansson 2.12 ](https://github.com/akheron/jansson/tree/v2.12)