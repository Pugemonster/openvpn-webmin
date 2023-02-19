# openvpn-webmin
OpenVPN Module for Webmin

This is the 3.3 version of the OpenVPN plugin for webmin.
Since the original development does not use a VCS i try to import new versions once in a while into this repository.

# Dev & Build

After doing changes, build module package by simply using tar

$ git clone https://github.com/Pugemon/openvpn-webmin.git .
$ ... apply your changes in openvpn/*
$ tar -cvzf openvpn.wbm.gz openvpn/

# Install

If you have a previous version running, remove it first:

- Login to Webmin interface
- Webmin > Webmin Configuration > Webmin Modules > Delete > OpenVPN + CA
- Remove the module configuration from /etc/webmin/openvpn/config

Now install the patched version:

- Login to Webmin interface.
- Webmin > Webmin Configuration > Webmin Modules > Install
- Click "From ftp or http URL"
- https://github.com/Pugemon/openvpn-webmin/raw/master/openvpn.wbm.gz
- Click "Install Module"
