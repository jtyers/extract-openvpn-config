# extract-openvpn-config
Extract individual parts of an OpenVPN (`*.ovpn`) config file.


Given a .ovpn file, this script will extract the pieces of that file into separate files;
this script will output new files with names based on the original file. So, for an original
.ovpn file named 'my-config.ovpn', this script will output:

```
	my-config.conf     # OpenVPN configuration file
	my-config.key.pem  # OpenVPN private key
	my-config.crt.pem  # OpenVPN certificate
	my-config.ca.pem   # OpenVPN CA certificate
```

usage: extract-openvpn-config <file.ovpn>
