# Guided-Exercise-Managing-Ansible-Project-Materials-Using-Git
Note : this exercice is a part of Red Hat automation with ansible course 

Clone an existing Git repository that contains an Ansible Playbook, make edits to files in that repository, commit the changes to your local repository, and push them to the original repository.

Outcomes


Clone a Git repository to the workstation machine.

Create a playbook to configure the Simple Network Management Protocol (SNMP) on Cisco IOS XE managed nodes.

Stage the playbook file, commit the changes, and synchronize with the remote repository.


As the student user on the workstation machine, use the lab command to prepare your environment for this exercise, and to ensure that all required resources are available. The command also removes any Simple Network Management Protocol (SNMP) configuration from the Cisco IOS XE managed nodes.

<img width="722" height="309" alt="image" src="https://github.com/user-attachments/assets/2b6e59af-9afa-409a-a33b-e8eb685a2874" />




**Instructions

Open a terminal and verify that SNMP is not configured on the iosxe1.lab.example.com managed node.

1) Connect to the iosxe1.lab.example.com managed node by using SSH:

<img width="707" height="171" alt="image" src="https://github.com/user-attachments/assets/c7a3def4-aef0-4459-a8a5-fb20d4848600" />

2) Display the SNMP configuration for the iosxe1.lab.example.com managed node. The command output indicates that the SNMP agent is not enabled:
   <img width="413" height="146" alt="image" src="https://github.com/user-attachments/assets/995fb19e-4031-4dd8-9975-24a6e6f6d058" />

3) Return to the workstation machine:
   <img width="556" height="101" alt="image" src="https://github.com/user-attachments/assets/2616149e-e04c-4da2-9ddc-c59b84b6e727" />

4) Clone the git@git.lab.example.com:student/snmp Git repository to the /home/student/git-repos directory. Create a branch named exercise and check out that branch.

Create the /home/student/git-repos directory if it does not exist, and then change to this directory:
<img width="420" height="69" alt="image" src="https://github.com/user-attachments/assets/de78604a-7acc-4019-82c5-a9db3378d6fd" />

Clone the git@git.lab.example.com:student/snmp repository, and then change to the repository directory:

<img width="692" height="171" alt="image" src="https://github.com/user-attachments/assets/c8b267cc-cd65-4a74-b24d-0f45b6c93b9b" />

Create and check out the exercise branch:

<img width="463" height="116" alt="image" src="https://github.com/user-attachments/assets/b087c5cb-e3d2-478f-871f-92501dabc72a" />

Note : You can also use the git checkout -b exercise command to create and check out the exercise branch by using a single command:



Open VS Code and create a playbook named cisco_snmp.yml in the /home/student/git-repos/snmp directory.

Open VS Code and click File → Open Folder. Navigate to Home → git-repos → snmp and then click Open.

<img width="962" height="718" alt="image" src="https://github.com/user-attachments/assets/970e6761-2770-443f-9bee-27eeb21822d3" />

In VS Code, click File → New Text File. Click Select a language and then click Ansible.

Create a playbook with the following content and save it as cisco_snmp.yml:

<img width="958" height="720" alt="image" src="https://github.com/user-attachments/assets/35ec62cc-7d92-44e8-9918-d5cc3c1d7ae7" />


In VS Code, stage and commit the SNMP playbook.

Click the Source Control icon in the left navigation menu, or click View → Source Control to display the Source Control panel.

Hover over your mouse over the file. A plus (+) symbol next to the file appears. Click the plus symbol to add the file to the Staged Changes section.

<img width="954" height="749" alt="image" src="https://github.com/user-attachments/assets/16a68943-c7f8-44e0-8e97-8c44f375bfe9" />

In the Message field in the Primary Side Bar, enter "Cisco SNMP playbook for IOS XE managed nodes" as the commit message and click Commit.

<img width="946" height="774" alt="image" src="https://github.com/user-attachments/assets/711dedda-432c-4e98-8a0f-90f005d213b8" />






