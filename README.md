## NAT Reflection

If you are running your nodes behind a NAT, i.e. port forwarding from your home router you probably don't have NAT reflection, its the ability to connect to your public IP from within your network, you can install the following tool to help with that 

#### Ubuntu

    sudo curl -sSL https://raw.githubusercontent.com/ctzoki/nat-reflection-hack/main/install-nat-reflection-ubuntu.sh | sudo bash

#### Usage

the tool supports 4 commands, add, list, reload, delete, add and delete take in two parameters public ip and private ip, run the add command to enable reflection for an ip

    sudo nat-reflection add {your-public-ip} {your-local-ip}

Add a reflection

    sudo nat-reflection list

List all reflections

    sudo nat-reflection reload

Reload, mostly used by the service on startup

    sudo nat-reflection delete {your-public-ip} {your-local-ip}

Delete a reflection, if you made a mistake or don't need it anymore
![image](https://github.com/ctzoki/neoxa-mn/assets/129646348/2682ee61-05af-4048-8e29-2de63bec2534)



