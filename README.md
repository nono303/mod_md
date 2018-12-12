# apache httpd mod_md windows builds #

----
- https://github.com/icing/mod_md
- https://httpd.apache.org/docs/trunk/mod/mod_md.html  

----
**V1.1.17-git + mod_ssl from httpd 2.4.37**  

> 2018-12-12 **IMPORTANT NOTE**
openssl dll **MUST be named libcrypto-1_1.dll and libssl-1_1.dll** in httpd /bin directory even for x64 (normally named libcrypto-1_1-x64.dll and libssl-1_1-x64.dll   
I will try to fix it ASAP *(see #3)*


2018-11-27 
 - pdb for so & dll
 - janson build dep 
 - curl build dep compiled with Winssl to avoid issue [#14](https://github.com/icing/mod_md/issues/14)  
    ```Enabled features: WinSSL libz AsynchDNS SSPI SPNEGO Kerberos NTLM```  
    ```Enabled protocols: DICT FILE FTP FTPS GOPHER HTTP HTTPS IMAP IMAPS LDAP POP3 POP3S RTSP SMTP SMTPS TELNET TFTP```

> - MSVC 15.9.2 / 19.16.27024.1
> - Window Kit 10.0.17134.0
> - **[AVX](https://msdn.microsoft.com/fr-fr/library/jj620901.aspx) build** __only for _avx directoy builds__
    
> - [Openssl 1.1.1a ](https://github.com/openssl/openssl/tree/OpenSSL_1_1_1a)  
> - [curl 7.62.0](https://github.com/curl/curl/tree/curl-7_62_0)  
> - [jansson 2.12 ](https://github.com/akheron/jansson/tree/v2.12)