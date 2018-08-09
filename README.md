# apache httpd mod_md windows builds #

----
@see  
- https://github.com/icing/mod_md
- https://httpd.apache.org/docs/trunk/mod/mod_md.html  

----
**V1.1.16-git + mod_ssl from httpd 2.4.34**  
2018-08-09 
 - curl 7.61 build dep compiled with Winssl to avoid issue [#14](https://github.com/icing/mod_md/issues/14)  
    ```Enabled features: WinSSL libz AsynchDNS SSPI SPNEGO Kerberos NTLM  ```  
    ```Enabled protocols: DICT FILE FTP FTPS GOPHER HTTP HTTPS IMAP IMAPS LDAP POP3 POP3S RTSP SMTP SMTPS TELNET TFTP```
 - janson build dep 
 - pdb for so & dll

Older version available on tags

[changelog](https://raw.githubusercontent.com/icing/mod_md/master/ChangeLog)

> - MSVC 15.7.5 / 19.14.26433
> - Window Kit 10.0.17134.0
    
> - [Openssl 1.1.0h ](https://github.com/openssl/openssl/tree/OpenSSL_1_1_0h)  
> - [curl 7.61.0](https://github.com/curl/curl/tree/curl-7_61_0)  
> - [jansson 2.11 ](https://github.com/akheron/jansson/tree/v2.11)