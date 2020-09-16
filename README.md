# Install_.NET_Agent
Playbook for Installation of .net Agent on windows server.

## Hosts file example
```bash
[win]
<target_name/ip>

[win:vars]
ansible_user=<windows_user>
ansible_password=<user_password>
ansible_connection=winrm
ansible_port=5985
```

## Run Example
```bash
ansible-playbook install_dotnetagent.yml -i <hosts file> -e "src=<msi_file_source> remote_src=<true (if the file is on the remote node)>"
```
