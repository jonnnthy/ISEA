# 1a-2 Ubuntu Desktop and Command Line Familiarisation

## Ubuntu Desktop GUI Familiarisation
- Check Internet using Firefox.
<img width="1916" height="1576" alt="firefox" src="https://github.com/user-attachments/assets/0570f632-9558-44ba-8a30-97ea1fe6ebb4" />

- Open LibreOffice and type a document.
<img width="1854" height="1408" alt="typing in libreoffice" src="https://github.com/user-attachments/assets/78892d49-27e5-4ed2-96a3-46e483bc5514" />

- Navigate directories using File Manager.
<img width="894" height="562" alt="file manager" src="https://github.com/user-attachments/assets/e1fdbac6-4499-4c51-9224-4fd8d9cfbf68" />

  
- Install a program via Ubuntu Software Centre.
<img width="1330" height="854" alt="installing libreoffice" src="https://github.com/user-attachments/assets/47da33e4-9551-407e-accf-7c8351ea830d" />

## CLI Basics and File Operations
- Use `ps -e`, `top`, and `1` to monitor processes.
<img width="864" height="578" alt="ps-e" src="https://github.com/user-attachments/assets/71262dfd-332c-42f5-b1d2-c365b74388b7" />

- Use `ls`, `ls -la`, `ls -alt`, `ls -lah` to explore files.
<img width="780" height="532" alt="ls-l-a" src="https://github.com/user-attachments/assets/b1559887-dd2e-41ca-aaaa-f5a126181e2a" />

- Create/edit/view files using `touch`, `gedit`, `nano`, `cat`.
<img width="292" height="74" alt="nano" src="https://github.com/user-attachments/assets/ea6d7241-952d-48d8-aaa8-75c3d171567a" />
<img width="388" height="66" alt="touch" src="https://github.com/user-attachments/assets/bb00d30b-914f-493a-ac63-e189cc082444" />
<img width="348" height="50" alt="cat" src="https://github.com/user-attachments/assets/471c769c-7a89-4b62-bc65-ee7de90dd6e2" />

- Copy and move files with `cp`, `mv`; delete with `rm`.
<img width="410" height="76" alt="mv" src="https://github.com/user-attachments/assets/46b893f6-0f1b-41f3-a947-af79c5b984bc" />
<img width="330" height="74" alt="rm" src="https://github.com/user-attachments/assets/180911e2-17df-479e-8e0d-365adca24488" />

## Super User and Permissions
- Use `whoami`, `sudo whoami` to demonstrate privilege escalation.
<img width="358" height="116" alt="whoami" src="https://github.com/user-attachments/assets/0005ab44-0661-4cab-9bd1-fffec48d68c2" />

## Network Configuration and DNS
- Use `ip a` to identify private IP.
<img width="1056" height="296" alt="ip a" src="https://github.com/user-attachments/assets/0fcbd715-cfd1-49e0-bbcd-ce929e47c6b0" />

- Ping local devices or 8.8.8.8.
<img width="576" height="116" alt="ping" src="https://github.com/user-attachments/assets/678ed003-6119-4bf4-a3a6-3a1ab440414c" />

- Use `nslookup` and install/use `whois` to investigate domains.
<img width="472" height="112" alt="nslookup" src="https://github.com/user-attachments/assets/feb282f2-5941-43cb-9090-72b7a1c07468" />

## Software Installation Methods
- Use `sudo apt update`, `sudo apt upgrade`, `sudo apt install vlc`.
<img width="1012" height="448" alt="sudo apt update" src="https://github.com/user-attachments/assets/96ea2688-cd43-4fa1-907d-5c42cfe0c6c6" />

## Reflection Questions
- Which file editors are best for remote access and why?
  
nano is best for remote access because it works in the terminal over SSH. GUI editors like gedit need a desktop environment.
  
- Compare software installation methods: SaaS vs binaries vs repos vs source.
  
SaaS runs online with no install. Binaries are manual installers. Repos (like apt) install from trusted package sources. Source means compiling the program yourself.

- What are pros/cons of each method from user and developer perspectives?
  
SaaS is convenient but needs internet. Binaries are easy but updates can be messy. Repos are safe and easy to update but may not be latest. Source is flexible but harder and time-consuming.
  
- How did using CLI improve your understanding of Linux?
  
CLI helped me understand file management, processes, networking, and software installation without relying on the GUI.
