# Cloud Web Server Deployment with Microsoft Azure

- Log in to Microsoft Azure and create a new Ubuntu 20.04 instance.
<img width="2618" height="554" alt="azure vm" src="https://github.com/user-attachments/assets/c038d5fc-dc88-41c5-bd83-6fb0d39b00ec" />



- Allow both SSH and HTTP traffic.
<img width="2986" height="576" alt="port rules" src="https://github.com/user-attachments/assets/8e10654d-ba0e-4361-89d7-bc1c90890495" />

- Connect to the VM using RDP.
<img width="3840" height="2114" alt="RDP to my cloud vm on XFCE" src="https://github.com/user-attachments/assets/5cf34ca7-23dc-4942-8561-763f941bfcfb" />

- Run `sudo apt update` and install Apache using `sudo apt install apache2`.
<img width="792" height="234" alt="Screenshot 2026-01-18 012930" src="https://github.com/user-attachments/assets/3ba41efc-39a8-4d0b-b34b-4d856f4b1aec" />


- Access the server using its public IP in a browser (via HTTP).
  <img width="1544" height="1384" alt="Screenshot 2026-01-09 210811" src="https://github.com/user-attachments/assets/10f39f1f-d686-478f-9a9e-72ff215e9fb2" />

- Modify `/var/www/html/index.html` using nano and test the changes live.
  <img width="1286" height="1266" alt="Screenshot 2026-01-09 204636" src="https://github.com/user-attachments/assets/a531f198-cdbc-4af3-a228-501d1348af2c" />
  
- Use `wget` to download remote files to your VM.
  <img width="1106" height="30" alt="wget" src="https://github.com/user-attachments/assets/3ea75f2e-79cc-46d8-ad2f-9494acc19b9c" />
  
- Use `scp -i key.pem localfile ubuntu@IP:/home/ubuntu/` to copy files from local to VM.
 <img width="1274" height="472" alt="sending my hello_world sh to my azure vm from local vm" src="https://github.com/user-attachments/assets/8f170acb-c6e1-43bd-8a56-449137bca16d" />

  

## Reflection Questions
- What were the benefits of cloud deployment over local virtualisation?

  
- How does Apache serve files, and how did you verify this?

  
- What did you learn about file ownership and permissions?

  
- What risks are associated with leaving instances running?

  
- How would you explain the difference between DNS and /etc/hosts to a client?
