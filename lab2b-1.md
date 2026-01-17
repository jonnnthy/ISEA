# Cloud Web Server Deployment with Microsoft Azure

- Log in to Microsoft Azure and create a new Ubuntu 20.04 instance.


- Allow both SSH and HTTP traffic.
  

- Connect to the VM using RDP.
 

- Run `sudo apt update` and install Apache using `sudo apt install apache2`.


- Access the server using its public IP in a browser (via HTTP).
  
- Modify `/var/www/html/index.html` using nano and test the changes live.
  
- Download and copy files to `/var/www/html/` using `wget` and `sudo cp`.
  
- Use `wget` to download remote files to your VM.
  
- Use `sudo cp` to move them into the web directory.
  
- Use `scp -i key.pem localfile ubuntu@IP:/home/ubuntu/` to copy files from local to VM.
 
  

## Reflection Questions
- What were the benefits of cloud deployment over local virtualisation?

  
- How does Apache serve files, and how did you verify this?

  
- What did you learn about file ownership and permissions?

  
- What risks are associated with leaving instances running?

  
- How would you explain the difference between DNS and /etc/hosts to a client?
