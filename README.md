# wgsd - wireguard service discovery

inspired by [jwhited/wgsd](https://github.com/jwhited/wgsd) but

- written in Python rather than in Go, using python modules available in Debian
- uses hostname for the instance name rather than base32 of the pubkey

`wgsd` creates the PTR/SRV/TXT/A records necessary to identify a wireguard node.

`wgsd-client` emits pubkey/port/address tuples resolved from the above records.
