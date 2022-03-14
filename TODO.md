* Set up backups trough restic
  * Backup to b2
  * Possibly some simple definitions to show where folders are located
  * Possible auto recovery on new installs?
    * Think about the steps to do a recovery from restic

* Set up grafana
  * Logging of minecraft
    * Hook into systemd logs
    * https://modrinth.com/mod/fabricexporter
    * https://modrinth.com/mod/serverstats
  * Figure out how to deal with logs and growing sizes
  * Set up some simple warnings like HDD/CPU spikes/RAM limits

* Figure out how to do run podman reliably trough ansible
  * Maybe use podman trough systemd
  * How are updates handled?

* Figure out if theres a nice way to get updatable components of system setup.
  * Podman
  * Apt
  * Minecraft
  * Minecraft Fabric mods
    * Github has some basic APIs, but seem annoying to use
    * Modrinth has good APIs, but would require a script to help
  * Where should there warnings go?
    * Should they repeat old out of date, or only warn about new out of date software?

* Look into a SSO/IDAP solution
  * Try Authentik or Keycloak
  * Use on
    * Grafana
