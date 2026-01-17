# Domain, DNS and TLS Certificates with Let's Encrypt

- Register a domain (Namecheap, GoDaddy, Cloudflare, Route 53, etc).
<img width="2988" height="2076" alt="duckdns" src="https://github.com/user-attachments/assets/8132a58e-891e-4a7f-8937-9e22ffb223b1" />

- Wait for DNS propagation and test with browser, ping, and nslookup.
<img width="2630" height="1736" alt="dnschecker" src="https://github.com/user-attachments/assets/8a7c6e4e-3755-427f-94b3-7aff36aeba07" />

- Install Certbot: `sudo apt install certbot python3-certbot-apache`.
<img width="1276" height="574" alt="installing certbot" src="https://github.com/user-attachments/assets/40ae54a3-dd8b-4f1a-b843-6e818c23a426" />

- Run: `sudo certbot --apache` to generate and install the certificate.
<img width="1280" height="178" alt="running certbot" src="https://github.com/user-attachments/assets/d01c1dc9-e2ae-4e8d-8624-8158bfbde415" />

- Check site: HTTPS lock icon should appear in browser.
<img width="664" height="594" alt="cert " src="https://github.com/user-attachments/assets/2694870d-dfd7-42f4-8eab-210c71b2a7ad" />


## Reflection Questions
- What is the role of DNS in Internet presence?

DNS maps a domain name to an IP address so users can reach your website.
  
- Why does DNS propagation take time?

Updates take time because DNS records are cached worldwide based on TTL values.

- How does Let’s Encrypt validate domain ownership?

It verifies you control the domain using HTTP challenges or DNS TXT record challenges.
  
- What are the risks if TLS is not configured on a public-facing site?
  
Data can be intercepted or altered, and users may see “Not Secure” warnings.
 
- What could happen if you leave your cloud VM running for months?
  
You may rack up costs and increase the chance of attacks or compromise.
