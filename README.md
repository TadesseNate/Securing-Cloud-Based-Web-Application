# Securing-Cloud-Based-Web-Application


<h2 style="font-size: 24px; text-align: center;"> Project Overview</h2>	



Enter the URL for the web application that you created:


https://tadessesecurity.azurewebsites.net/
	

Paste screenshots of your website created:

![image4](https://github.com/user-attachments/assets/6e3f0e20-ce59-4f38-b2fc-574ff7520dea)



![image1](https://github.com/user-attachments/assets/84c6497d-95f0-405d-8dbb-ea9ae6b628fd)



General Questions


1. What option did you select for your domain (Azure free domain,  GoDaddy domain)?

I selected Azure free domain
	

2. What is your domain name?

tadessesecurity.azurewebsites.net
	

<h2 style="font-size: 24px; text-align: center;"> Networking Questions</h2>



1. What is the IP address of your webpage?


20.211.64.11
	

2. What is the location (city, state, country) of your IP address?


Australia East 
	

3. Run a DNS lookup on your website. What does the NS record show?


  ![image2](https://github.com/user-attachments/assets/c4c23d0e-110b-446d-8b64-4173b264da82)


	
<h2 style="font-size: 24px; text-align: center;"> Web Development Questions</h2>



1. When creating your web app, you selected a runtime stack.  What was it? Does it work on the front end or the back end? 


Runtime stack selected was PHP 8.2 and works on the back end. 
	

2. Inside the /var/www/html directory, there was another directory called assets. Explain what was inside that directory.


The assets directory is a collection of crucial resources for the front-end of a web application, ensuring its user-friendly functionality.
	

3. Consider your response to the above question. Does this work with the front end or back end?


Front-end
	






<h2 style="font-size: 24px; text-align: center;"> Cloud Questions</h2>


1. What is a cloud tenant?


A cloud tenant utilizes a shared cloud environment, gaining cost savings, scalability, and reduced management overhead while maintaining secure and isolated operations.
	

2. Why would an access policy be important on a key vault?


An access policy is crucial for maintaining security and preventing unauthorized access to a key vault.
	

3. Within the key vault, what are the differences between keys, secrets, and certificates?


Keys are utilized for cryptographic operations, secrets are used to store sensitive data, and certificates are used to secure communications and verify identities.
	




<h2 style="font-size: 24px; text-align: center;"> Cryptography Questions</h2>



1. What are the advantages of a self-signed certificate?


Self-signed certificates offer cost savings, immediate availability, full control over certificate properties, ideal for non-production environments, private networks, educational purposes, and flexibility, with no dependency on external entities and custom expiration dates.
	









2. What are the disadvantages of a self-signed certificate?


Self-signed certificates lack public trust, leading to security warnings and distrust. They are vulnerable to MITM attacks and lack revocation. They require manual distribution and maintenance, making them unsuitable for public websites. They can harm an organization's professional image. They also lack third-party validation, identity assurance, and insurance. Trusted Certificate Authorities (CAs) offer warranties in case of certificate-related security breaches, which self-signed certificates lack. Therefore, they are not suitable for public websites or applications.
	

3. What is a wildcard certificate?


A wildcard certificate simplifies domain and first-level subdomain security with a single certificate, but requires careful handling of security and management considerations.
	

4. When binding a certificate to your website, Azure only provides TLS versions 1.0, 1.1, and 1.2.  Explain why SSL 3.0 isn’t provided.


Azure does not offer SSL 3.0 certificates for website binding due to identified security vulnerabilities in the SSL 3.0 protocol.
	

5. After completing the Day 2 activities, view your SSL certificate and answer the following questions:


   1. Is your browser returning an error for your SSL certificate? Why or why not?


yes, open ssl certificate
	

   2. What is the validity of your certificate (date range)?


Issued On
Friday, May 17, 2024 at 10:59:33 AM
Expires On
Sunday, May 17, 2026 at 10:59:33 AM


Issued On
Tuesday, March 12, 2024 at 6:36:42 PM
Expires On
Friday, March 7, 2025 at 5:36:42 PM


	

   3. Do you have an intermediate certificate? If so, what is it?


Certificate
b5aaee06535a5be7b8f97ba8246c04d00b8c5a067c7d90e4bba96dcfcbd79062


Certificate
69ff299d956c85b15be96f2f39e9d4b91dfa17bb075bc34507dc1628c294314f


	

   4. Do you have a root certificate? If so, what is it?


DigiCert Global Root G2
*.badssl.com
	

   5. Does your browser have the root certificate in its root store?


yes, PKCS #1 SHA-256 With RSA Encryption
	

   6. List one other root CA in your browser’s root store.


PKCS #1 SHA-256 With RSA Encryption
	





<h2 style="font-size: 24px; text-align: center;"> Cloud Security Questions</h2>




1. What are the similarities and differences between Azure Web Application Gateway and Azure Front Door?


Azure Web Application Gateway and Azure Front Door are distinct Azure ecosystem roles, with Web Application Gateway focusing on regional application delivery and security, and Front Door providing global performance optimization.
	

2. What is SSL offloading? What are its benefits?


SSL offloading is the process of decrypting SSL/TLS-encrypted traffic at a dedicated device, preventing it from being forwarded to backend servers in plaintext.
	

3. What OSI layer does a WAF work on?


 A Web Application Firewall (WAF) operates at Layer 7 of the OSI model, ensuring comprehensive security by inspecting, monitoring, and filtering HTTP/HTTPS traffic.
	

4. Select one of the WAF managed rules (e.g., directory traversal, SQL injection, etc.), and define it.


Command Injection Protection is a crucial rule in a Web Application Firewall that detects and blocks unauthorized commands, preventing severe security breaches caused by web application vulnerabilities.
	

5. Consider the rule that you selected. Could your website (as it is currently designed) be impacted by this vulnerability if Front Door wasn’t enabled? Why or why not?


If Azure Front Door isn't enabled, your website can be vulnerable to command injection vulnerabilities if it doesn't properly validate user inputs or blocks attempts.
	

6. Hypothetically, say that you create a custom WAF rule to block all traffic from Canada. Does that mean that anyone who resides in Canada would not be able to access your website? Why or why not? 


Yes,custom WAF rules can block Canadian traffic from a website, preventing users from accessing it unless they use VPNs or proxies to mask their true location.
	

7. Include screenshots below to demonstrate that your web app has the following:


   1. A WAF custom rule
  ![image5](https://github.com/user-attachments/assets/94ad7695-7f3d-4c39-b2c4-88c9ab89b8d8)


	


