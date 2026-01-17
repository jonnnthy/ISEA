# Linux File Permissions and Group Access Control

- Create users: `sudo adduser alice`, `sudo adduser bob`, `sudo adduser mallory`.
<img width="520" height="28" alt="Screenshot 2026-01-17 224900" src="https://github.com/user-attachments/assets/fd75784b-4948-4b17-9942-9740d09f2ddf" />
<img width="754" height="50" alt="bob" src="https://github.com/user-attachments/assets/e403725a-5f60-4147-b628-01b90957dcd1" />
<img width="768" height="50" alt="mallory" src="https://github.com/user-attachments/assets/f4cc060d-4ce0-441b-807f-f98d50cade54" />

- Create a group: `sudo groupadd sharedgroup`.
<img width="512" height="74" alt="groupadd sharedgroup" src="https://github.com/user-attachments/assets/aa031875-1ff5-4b51-9643-ce75ce6a7ecf" />

- Create a directory: `sudo mkdir /home/shared`.
<img width="548" height="70" alt="mkdir" src="https://github.com/user-attachments/assets/2a9bba1c-4828-4366-b48d-fba3178e988f" />

- Create ten files inside it: `sudo touch /home/shared/file{1..10}`.
<img width="640" height="288" alt="create 10 files" src="https://github.com/user-attachments/assets/adb07a77-54cc-46dd-88f0-7eb057fc5d62" />

- Change group ownership: `sudo chgrp -R sharedgroup /home/shared`.
<img width="668" height="338" alt="change group ownership" src="https://github.com/user-attachments/assets/3578773b-6aa2-4407-ac02-d093f1338c3b" />

- Add Alice and Bob to group: `sudo usermod -aG sharedgroup alice`, `sudo usermod -aG sharedgroup bob`.
<img width="592" height="132" alt="add alice bob into group" src="https://github.com/user-attachments/assets/5a30c600-19eb-4e3a-b7dd-0f430255a5b6" />

- Set directory permissions: `sudo chmod -R 770 /home/shared`.
<img width="658" height="70" alt="chmod 770" src="https://github.com/user-attachments/assets/5e160a0b-094e-4b80-b7ba-de4d0bf328fe" />

- Override Bob's rights: `sudo chmod 750 /home/shared/*`.
<img width="546" height="22" alt="750" src="https://github.com/user-attachments/assets/f9369d6a-074f-4f3c-9bc7-410a74d23adf" />

- Remove Mallory from any group with access.
<img width="384" height="48" alt="mallory no group" src="https://github.com/user-attachments/assets/9bf3b407-ebec-42cb-8c33-229b84948af9" />

- Switch user: `su - alice`, `su - bob`, `su - mallory`; use `whoami` and `ls -l /home/shared` to verify access.
<img width="550" height="356" alt="change user" src="https://github.com/user-attachments/assets/0beb5a6b-ad7f-4eca-a2bb-5b628d174689" />

## Reflection Questions
- How do Linux permissions differ from Windows ACL?

Linux uses simple owner/group/others permissions, while Windows ACLs allow more detailed per-user/per-group rules.

- What’s the effect of chmod 770 vs 750?

770 gives full access to owner and group. 750 gives full access to owner but only read/execute to group (no write).

- What is the risk of adding users to the sudo group?

They can run admin commands, so mistakes or compromised accounts can affect the whole system.

- Why is it important to verify with `su` and `whoami`?

It confirms you’re testing as the correct user and proves the permissions work as intended.
