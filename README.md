# How to netinstall debian using a custom pressed using the netinst iso

- Serve the preseed file via python's http.server module `python -m http.server 9000`
- Boot with netinst.iso
- Select Advanced Options
- Press tab on automated install
- Add the following before `--- quiet`, `interface=eth0 net.ifnames=0 hostname=gw`
- When the install process asks for the location of the preseed file
  `http://<ip address>:<port>/preseed.cfg`
# preseeds
