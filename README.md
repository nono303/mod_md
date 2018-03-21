# apache httpd mod_md windows builds #

----
@see  
- https://github.com/icing/mod_md
- https://httpd.apache.org/docs/trunk/mod/mod_md.html  
- https://www.apachelounge.com/viewtopic.php?t=7786  

----
**V1.1.10-git + mod_ssl from httpd 2.4.33**  
2018-03-21 
 - curl 7.59**build dep compiled with Winssl to avoid issue [#14](https://github.com/icing/mod_md/issues/14)  
    ```Enabled features: WinSSL libz AsynchDNS SSPI SPNEGO Kerberos NTLM  ```  
    ```Enabled protocols: DICT FILE FTP FTPS GOPHER HTTP HTTPS IMAP IMAPS LDAP POP3 POP3S RTSP SMTP SMTPS TELNET TFTP```
 - janson build dep 
 - pdb for so & dll

Older version available on tags

[changelog](https://raw.githubusercontent.com/icing/mod_md/master/ChangeLog)

> - MSVC 15.6.3  
> - Window Kit 10.0.16299.0    
    
> - [Openssl 1.1.0g ](https://github.com/openssl/openssl/tree/OpenSSL_1_1_0g)  
> - [curl 7.59.0](https://github.com/curl/curl/tree/curl-7_59_0)  
> - [jansson 2.11 ](https://github.com/akheron/jansson/tree/v2.11)