# Root Interview Demo with Ansible

## Creating EC2 Server
Create an Ubuntu Server 20.04 LTS (HVM)

The default settings are fine but make sure your security group has TCP ports 22 & 4567 open for your IP

Once the instance is running ssh in and run the following command:

```shell
sudo apt update; sudo apt install -y ansible git; ansible-pull -U https://github.com/lirebotes/root root_playbook.yaml
```
Once Ansible finishes you should be able to able to run “curl http://[hostip]:4567”
