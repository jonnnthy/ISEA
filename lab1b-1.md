# 1b-1 Linux Services, SSH, Firewalls & Compression

- Install Apache using `sudo apt install apache2` and test `http://127.0.0.1`.
<img width="1544" height="1384" alt="Screenshot 2026-01-09 210811" src="https://github.com/user-attachments/assets/67611683-f4f5-4a0d-b513-270c179e6554" />

- Install SSH server and Nmap: `sudo apt install openssh-server nmap`.
<img width="840" height="250" alt="installing nmap" src="https://github.com/user-attachments/assets/76a8378a-4881-47cd-9acc-78b63a21ca11" />

- Scan each other's ports using `nmap [IP]` and note open services.
<img width="814" height="358" alt="nmap open ports on my azure VM" src="https://github.com/user-attachments/assets/65359eb2-2c0f-4e22-8bc2-0034771ea277" />

- Determine IP using `ip a` and visit peer web page in browser.
<img width="612" height="361" alt="image" src="https://github.com/user-attachments/assets/a5f6c3a3-73f8-47c7-9a29-916d0a0c4134" />

- Enable UFW with `sudo ufw enable`, allow port 80, and observe service access.
<img width="554" height="114" alt="ufw enable port 80" src="https://github.com/user-attachments/assets/ee1f1772-87b2-4838-8289-2370947bf2c5" />

- Download books from Project Gutenberg using `wget`.
<img width="1106" height="30" alt="wget" src="https://github.com/user-attachments/assets/a8d32357-bbcd-48f8-bcfb-0ecf7c6cd4da" />

- SSH into your partner’s machine and create a file on their Desktop.
<img width="1708" height="1230" alt="creating a text file using SSH" src="https://github.com/user-attachments/assets/220f5266-0d02-49b9-91c9-1c90ec1ad73c" />

- Use `scp file.txt user@host:/destination/` to send a file over the network.
<img width="1274" height="472" alt="sending my hello_world sh to my azure vm from local vm" src="https://github.com/user-attachments/assets/2bca85f9-5fc5-479e-a4d0-b6fdbf0f5227" />

## Reflection Questions
- What’s the role of a firewall in managing services?
It controls which ports/services are allowed or blocked, reducing unnecessary access and improving security.
  
- How did SSH access deepen your understanding of Linux as a server?
It showed me how Linux can be managed remotely through the terminal without needing a GUI.
  
- Why is file compression important in server contexts?
It saves storage space and makes file transfers faster and more efficient.
  
- How does user privilege management help secure systems?
It limits what users can do, preventing accidental changes and reducing the impact of attacks.
