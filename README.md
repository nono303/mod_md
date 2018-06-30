# apache httpd mod_md windows builds #

----
@see  
- https://github.com/icing/mod_md
- https://httpd.apache.org/docs/trunk/mod/mod_md.html  

----
**V1.1.13-git + mod_ssl from httpd 2.4.33**  
2018-06-30 
 - curl 7.60 build dep compiled with Winssl to avoid issue [#14](https://github.com/icing/mod_md/issues/14)  
    ```Enabled features: WinSSL libz AsynchDNS SSPI SPNEGO Kerberos NTLM  ```  
    ```Enabled protocols: DICT FILE FTP FTPS GOPHER HTTP HTTPS IMAP IMAPS LDAP POP3 POP3S RTSP SMTP SMTPS TELNET TFTP```
 - janson build dep 
 - pdb for so & dll

Older version available on tags

[changelog](https://raw.githubusercontent.com/icing/mod_md/master/ChangeLog)

> - MSVC 15.7.4 / 19.14.26431
> - Window Kit 10.0.17134.0
    
> - [Openssl 1.1.0h ](https://github.com/openssl/openssl/tree/OpenSSL_1_1_0h)  
> - [curl 7.60.0](https://github.com/curl/curl/tree/curl-7_60_0)  
> - [jansson 2.11 ](https://github.com/akheron/jansson/tree/v2.11)
