Using Existing Technologies to Make the Web More Secure

While exploring new ideas for adding security to Internet protocols and Web formats nad languages, it's useful to examine what current mechanisms exist to add security to existing Web transactions.  The following practices are currently being used on some high-volume production Web sites, but the whole Web would benefit from their adoption in more places and in more scenarios, especially when confidentiality is desirable.  Currently some of these techniques may not have come into wide use due to cost to implement or a perception that the majority of users are using browsers that do not support them.  However, with the increased industry attention on security and anti-snooping, and considerting that most modern browsers have implemented these techniques, adoption should be widely encouraged.

Recommendations from the TAG on How to Make the Web More Secure

The [http://www.w3.org/2001/tag/2013/10/whiteboard-security.jpg](list from our f2f meeting in Cambridge Mass) was:

1. Perfect Forward Secrecy over HTTPS

Perfect forward secrecy is a techinque which employees a different public key for each session.  That means that if an attacker breaks or obtains a key they can only decrypt the traffic of that session.  (need stable reference)

2. Key Strength

3. Certificate Pinning

As described [https://www.owasp.org/index.php/Certificate_and_Public_Key_Pinning here], cerfificate pinning is the process of associating a host with their expected X509 certificate or public key.

4. Versions

Up-to-date versions of security algorithms should always be employed.

5. HSTS

[http://tools.ietf.org/html/rfc6797 HTTP Strict Transport Security] is a proposed approach for web sites to declare that they may only be accessed via secure connections. 

6. Emplploy Encryptions in More Cases (“Crypto all the things”)

Increasingly any Web site can be handling privacy-comprimising information.  When we talk about securing communication over the web, some applications that spring to mind are financial transactions, social networks, messaging.  However, with advanced Web APIs, any Web site can requesting a users' location (for example to provide them peronalized directions), or request access to the user's microphone or camera (for example, connect a user with a customer services agent).  This means an increasing percentage of Web traffic can include personal or private information is on the increase.  In this environment it makes sens for Web sites to move more of their traffic behind ecrypted connections.

