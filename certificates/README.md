#  How to Install an SSL Certificate


An SSL Certificate is a text file with encrypted data that you install on your server so that you can secure/encrypt 
sensitive communications between your site and your customers via the Browser.

After you create a CSR (certificate signing request) and purchase a certificate, the issuer's 
validation team validates and processes your certificate request. Once validated, 
an SSL Certificate is sent to you via email. You can also download your SSL Certificate in your DigiCert account.

After you’ve installed your SSL Certificate, it is recommended that you make a backup copy of the certificate
and store it in a secure place. If a server crashes or needs to be replaced, 
it is much easier to secure the replacement server.

When downloading your SSL Certificate from your account, you will need to download an intermediate certificate. 
Browsers require the intermediate certificate to complete the certificate trust chain. The intermediate certificate links your SSL Certificate to DigiCert’s root certificate. 

Registered Certificate Authorities such as for example DigiCert must provide a known root certificate before their SSL Certificate can be trusted by SSL-enabled applications. With some servers such as Microsoft, the intermediate certificates are bundled with the SSL Certificate.

Once you have your certificate installed, it is recommended that you check that everything is working correctly using an SSL Installation Diagnostics or Inspector Tool. 



<!-- 
####

#####  
 -->

