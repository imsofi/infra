## Backup strategy:

Folders:
* `/opt/minecraft/worlds/{{ minecraft_server_name }}`

Pre Backup:
* Ledger respects save strategies. So this is simple:
* `echo 'save-off' > /run/minecraft-{{ minecraft_server_name }}/console`

Post Backup:
* `echo 'save-on > /run/minecraft-{{ minecraft_server_name }}/console'`
