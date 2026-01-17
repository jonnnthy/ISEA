# File Search, Analysis & Archiving in Linux

- Download `gutenberg.tar.bz2` from LMS.
<img width="494" height="48" alt="download gutenberg" src="https://github.com/user-attachments/assets/931c9a0d-da47-4695-860f-54750574e312" />

- Extract with: `bunzip2 gutenberg.tar.bz2` then `tar -xvf gutenberg.tar`.
<img width="586" height="210" alt="extract gutenberg tar" src="https://github.com/user-attachments/assets/6f379174-a019-4545-93ac-f4861ea73807" />

- Explore contents: `ls -l`, `tree`, or use `less` to inspect a few files.
<img width="338" height="140" alt="tree" src="https://github.com/user-attachments/assets/e68a5b98-c169-4e99-8074-acb21cf9db0b" />
<img width="208" height="88" alt="less moby txt" src="https://github.com/user-attachments/assets/3dc25f0d-ed4b-44a0-b0e7-62bc70f1c27d" />

- Search for filenames: `find ./Gutenberg -name "*.txt"`.
<img width="474" height="92" alt="find" src="https://github.com/user-attachments/assets/e684c84b-5fe4-4573-b683-3adc19125f28" />

- Search for strings: `grep -r 'keyword' ./Gutenberg` or use `find -exec grep`.
<img width="454" height="46" alt="grep" src="https://github.com/user-attachments/assets/02c81199-aca2-4458-adeb-8cc3e09b8a3d" />

- Search with context: `grep -r -C 3 'Next day' ./Gutenberg`.
<img width="606" height="28" alt="grep next day" src="https://github.com/user-attachments/assets/25761a7e-5478-4c69-bc47-7ecca9aebd78" />

- Find largest files: `du -a ./Gutenberg | sort -nr | head`.
<img width="630" height="114" alt="largest file" src="https://github.com/user-attachments/assets/1065e2a0-1f3f-4b74-a797-5e7b30dd5414" />

## Reflection Questions
- Which command-line tool was the most useful in solving the questions?

find was the most useful because it quickly locates files by name, size, and type.
  
- How might these search tools help in cybersecurity investigations?
  
They help identify suspicious files, search for keywords, and quickly review logs or evidence during incident response.
  
- How could scripting improve repetitive search tasks?

Scripts can automate repeated searches, save time, and produce consistent results across many folders and systems.
  
- What limitations did you encounter using grep and find?
  
grep output can be messy on large datasets, and find commands can be hard to remember and easy to type wrongly without practice.
