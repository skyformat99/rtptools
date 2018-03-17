# RTP Tools

RTP Tools is a set of small applications
that can be used for processing RTP data.
Refer to the individual manpages for details.

* **rtpplay**
	play back RTP sessions recorded by rtpdump
* **rtpsend**
	generate RTP packets from textual description,
	generated by hand or rtpdump
* **rtpdump**
	parse and print RTP packets,
	generating output files suitable for rtpplay and rtpsend
* **rtptrans**
	RTP translator between unicast and multicast networks
* **multidump**
	Start multiple rtpdumps simultaneously.
* **multiplay**
	Start multiple rtpplays simultaneously.

## Installation

The RTP tools should compile on any POSIX-compliant
platform supporting sockets.

- If building from git, run the following first to regenerate the build tools:

```
aclocal
automake --add-missing --force-missing
autoconf
```

- Run `./configure` to configure rtptools for your system.
- Run `make` to build rtptools.
- Run `make install` to install.
- Run `make uninstall` to uninstall.
- Run `make rpm` to create a rpm package. The rpm files will be in ./rpmbuild/RPMS.


## TODO

* Fix type mismatch warnings.
* Fix building on windows.
* Generate a Debian package.
