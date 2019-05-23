## <b>Ansible</b> 

- Ansible and its modules are written in Python

- use SSH to establish sessions

- Agentless

---

  #### Playbook

file in YAML that instruct Ansible on what to do

##### Task

define operation to be performed in the destination host

##### Inventory

host file in INI format

>  /etc/ansible/hosts

##### Role

A collection of tasks. useful for run a subset of tasks multiple times from different playbooks

---

#### Setup Environment

- Ubuntu

- Centos/Fedora

- MacOSX

<code>pip install ansible</code>

---

#### Config

> ansible.cfg

Find .cfg sequentially in current directory --> home --> /etc/ansible/ansible.cfg

---

### YAML formart

#### host

*Only group can be used*

<code>all</code>

target all host in inventory file 

or 

using the __group name__ stated in the INI file

#### connection

<code> local</code>

running Ansible without SSH

#### task

Format for a task:

<code>- module_name: parameter1=value parameterX=value</code>

---

### Run Playbook

<code>ansible-playbook name.yml</code>



> PLAY [host]************************....
>
> GATHERING FACTS *******.....
>
> TASK: [task]*******......
>
> PLAY RECAP *******....
>



play:	 					targeting all hosts

gathering facts: 	collecting  information from the host

task: 						The task is running. and the output of each host the task		

play recap: 			 showing the number of tasks in host resulting in ok, changed, unreachable and failed



---

### Apply Remote Control

##### control host 

the machine running Ansible

##### remote host

the remoted machine, need to have SSH and Python installed 



#### Configure SSH keys







---

References:

<https://medium.com/@denot/ansible-101-d6dc9f86df0a>



Typed by Percy Chau 22-5-2019*












