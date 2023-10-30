# VM Setup Continued (REQUIRED)
Truffle v4.0.4 which is installed on the VM is outdated and will provide this error if you proceed with the instructions without performing the updates:
![[Pasted image 20231031000241.png]]# **Steps to update Truffle:**

1. Run `sudo npm install -g truffle@4.1.15` (You will need to provide the system password which is **ubuntu**).
![[Pasted image 20231031000306.png]]

2. Run `sudo cp ./.npm-global/bin/truffle /usr/bin/truffle`

3. Truffle should be updated to v4.1.15. You can check the version by typing truffle version![[Pasted image 20231031000328.png]]
For some reason, doing Step 1 alone installs Truffle to a different directory than the one for normal commands, so we copy it in Step 2 to the Environment Variables folder (not necessary to know for this course).