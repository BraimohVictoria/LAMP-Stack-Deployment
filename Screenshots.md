How to Automate a LAMP Stack (Linux, Apache, MySQL, PHP) Using Bash Script and Ansible

Goal: At the end of tthis task, you will be able to host the Laravel website on a slave machine.

Step 1: Provision your master and slave machines in the vagrant configuration file. Here, the master node is called "Master" while the slave node is called "Node"
![](./Exam_Screenshots/Cloud_Exam%201.png)
Step 2: Run vagrant using the command 'sudo vagrant up' to prevent 'permission denied' issues. This command will set up your master node and slave node automatically.![](./Exam_Screenshots/Cloud_Exam%202.png)
Step 3: Go into the master machine using the command 'sudo vagrant ssh master'. Create your bash script file with the command 'touch.sh'![](./Exam_Screenshots/Cloud_Exam%203.png)
Step 4: Use the nano text editor to write the script. Your bash script should contain all your installations. The MySQL database, PhP, Apache2 Save and exit.![](./Exam_Screenshots/Cloud_Exam%204.png)
Step 5: Still in the master node, create an ansible folder or directory. In this folder, create your inventory and playbook files.![](./Exam_Screenshots/Cloud_Exam%205.png)
Step 6: Using your nano text editor, write your inventory. Your inventory in this case is the list of your machines and their ip addresses. (Master and Slave). ![](./Exam_Screenshots/Cloud_Exam%206.png)
Step 7: Write your playbook. This will automatically reflect on your slave node when it runs.![](./Exam_Screenshots/Cloud_Exam%207.png)
Step 8: Generate your ssh key to allow you connect to the slave node or machine.![](./Exam_Screenshots/Cloud_Exam%208.png)
Step 9: This is what your ssh key looks like. Copy this key and save in your slave node.![](./Exam_Screenshots/Cloud_Exam%209.png)
Step 10: In your slave node, use the nano edit to save the ssh key you copied from the master node to your authorized keys.![](./Exam_Screenshots/Cloud_Exam%2010.png)
Step 11: Go back to your master node and ping the ip addresses in your inventory.![](./Exam_Screenshots/Cloud_Exam%2011.png)
Step 12: Run your playbook.![](./Exam_Screenshots/Cloud_Exam%2012.png)
Step 13: Copy the ip address of your slave node and paste on your browser. The image below will be your result![](./Exam_Screenshots/Cloud_Exam%2013.png)
Congratulatiions! You just successfully hosted the Laravel website on your machine uusing a LAMP Stack.