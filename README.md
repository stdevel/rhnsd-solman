rhnsd-solman
============

SMF Manifest for Red Hat Network daemon on Solaris-like operating systems

This manifest starts RHNSD with a 10 minute interval (--interval=10) after establishing the network connectivity. You might want to change this value before importing and enabling the service:

```
# wget https://raw.githubusercontent.com/stdevel/rhnsd-solman/master/rhnsd.xml
# svccfg validate rhnsd.xml
# svccfg import rhnsd.xml
# svcadm enable rhnsd
```
