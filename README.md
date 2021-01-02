# armbian-aml-arm64-buster
Mirror for the latest build of Armbian for Amlogic arm64 SoCs (Debian Buster) Built by @150balbes

## Known issues:

"sudo" breaks after a while.

Fix:

  chown root:root /usr/bin/sudo 
  chmod 4755 /usr/bin/sudo
  chown root:root /usr/lib/sudo/sudoers.so 
  chmod 4755 /usr/lib/sudo/sudoers.so
  chown root:root /etc/sudoers
  chown root:root /etc/sudoers.d /etc/sudoers.d/README  /var/lib/sudo

Or keep using sudo only through ctrl + alt + f3 / ssh
