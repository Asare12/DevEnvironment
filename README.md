# DevEnvironment

## Setting up vagrant file
-Inside directory, create file called Vagrantfile with contents:
```
Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64" 
  config.vm.network "private_network", ip: "192.168.10.100"
  
  end

```


## Vagrant commands
- `vagrant up` Launches the VM
- `vagrant status` Views status of the VM
- `vagrant ssh` SSH's into the VM
- 

## VM Commands
- Update VM `sudo apt-get update -y` (sudo runs with perms, apt-get is an install manager, -y flag accepts all permissions.) 
- Install a program `sudo apt-get install {program}` 
- e.g., `sudo apt-get install nginx`


## Verify nginx 
- Open browser and navigate to 192.168.10.100
- The nginx splash page should be visible.

