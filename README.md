# apache httpd mod_md windows builds #

----
@see  
- https://github.com/icing/mod_md
- https://httpd.apache.org/docs/trunk/mod/mod_md.html  
- https://www.apachelounge.com/viewtopic.php?t=7786  

----
**V1.1.8 + [mod_ssl patched](https://github.com/icing/mod_md/blob/master/patches/mod_ssl_md-2.4.x-v5.diff) for it**  
2018-01-20 
 - curl build dep compiled with Winssl to avoid issue [#14](https://github.com/icing/mod_md/issues/14)  
    ```Enabled features: WinSSL libz AsynchDNS SSPI SPNEGO Kerberos NTLM  ```  
    ```Enabled protocols: DICT FILE FTP FTPS GOPHER HTTP HTTPS IMAP IMAPS LDAP POP3 POP3S RTSP SMTP SMTPS TELNET TFTP```
 - janson build dep 
 - pdb for so & dll

Older version available on tags

[changelog](https://raw.githubusercontent.com/icing/mod_md/master/ChangeLog)

> - MSVC 15.5.4  
> - Window Kit 10.0.16299.0    
    
> - [Openssl 1.1.0g ](https://github.com/openssl/openssl/tree/OpenSSL_1_1_0g)  
> - [curl 7.57.0](https://github.com/curl/curl/tree/curl-7_57_0)  
> - [jansson 2.10 ](https://github.com/akheron/jansson/tree/v2.10)