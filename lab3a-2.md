# Enabling HTTPS with Let's Encrypt & Certbot

- Firewall allows ports 22 (SSH), 80 (HTTP), 443 (HTTPS).
<img width="556" height="298" alt="ufw status" src="https://github.com/user-attachments/assets/112256a3-e4a8-412a-9973-8385415deb74" />

- Run: `sudo certbot --apache` and follow the prompts.
<img width="1280" height="178" alt="running certbot" src="https://github.com/user-attachments/assets/3f29cb20-6b75-4aa8-8e58-568adb414d03" />

- Click the lock icon to view certificate details (issuer, expiry, etc.)
<img width="664" height="594" alt="cert " src="https://github.com/user-attachments/assets/de98c6f5-5e84-45f4-8bde-e38a60e6ed1f" />

## Reflection Questions
- Why is HTTPS important for modern web applications?

It encrypts data in transit, prevents tampering, and builds user trust.
  
- What entity issued your site’s TLS certificate?

Let’s Encrypt.

- How long is your certificate valid for, and how can it be renewed?

90 days, and it can be renewed automatically using Certbot renewal.
  
- What happens if a certificate expires and is not renewed?

Browsers will warn users and the site may be blocked or seen as unsafe.
  
- Why does Let’s Encrypt require port 80 or 443 to be open for verification?

So it can reach your server to confirm you control the domain via HTTP/HTTPS challenge.  
