# ansible-101-control-machine

## *nix (Mac, Linux...)

### Step 1.
Install [Virtualbox](https://www.virtualbox.org/wiki/Downloads)

### Step 2.
Install [Vagrant](http://www.vagrantup.com/downloads)

### Step 3.
Install [Ansible](http://docs.ansible.com/ansible/intro_installation.html)

### Verification.

- Clone/download the [workshop repository](https://github.com/penguinjournals/ansible-101)
- From inside task1 folder run "vagrant up" (you'll need internet in this step)
- When the machine has started up run "ansible all ping", you should get this:
```
task1 | success >> {
    "changed": false,
    "ping": "pong"
}
``` 
If you get some error like:

`task1 | FAILED => private_key_file (./insecure_private_key) is group-readable or world-readable and thus insecure - you will probably get an SSH failure`

Run:

chmod 400 insecure_private_key

## Windows

### Step 1.
Install [Virtualbox](https://www.virtualbox.org/wiki/Downloads)

We'll use it for creating and destroying virtual machines on your computer easily.

### Step 2.
Install [Vagrant](http://www.vagrantup.com/downloads)

The machines we'll use during the workshop will be created and managed using vagrant.

### Step 3.
Clone/download this repository to your computer

### Step 4.
Run "vagrant up" from the root folder of the repository (*)

### Step 5.
Now you can connect to the machine using:

vagrant ssh


Once you are inside the virtual machine you should do:

cd /vagrant

git clone https://github.com/penguinjournals/ansible-101.git
