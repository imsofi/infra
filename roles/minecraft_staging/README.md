## Backup strategy:

Folders:
* `/opt/minecraft/worlds/prod`

Pre Backup:
* Ledger respects save strategies. So this is simple:
* `echo 'save-off' > /run/minecraft-prod/console`

Post Backup:
* `echo 'save-on > /run/minecraft-prod/console'`
