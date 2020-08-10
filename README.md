# shepd-dns
SHEPD is a cloud-based service that filters your DNS traffic according to your rules, protecting your applications and cloud infrastructure from outbound traffic to malicious sites, get forewarning of instances behaving suspiciously and, through SHEPD caching, gain performnace.

Requires a free account at https://shepd.io/ to get started.

## Installation

Currently `shepd-dns` is distributed in DEB package format, compatible with Ubuntu and Debian. The package is designed to be as self-standing as possible, with no dependencies beyond the base system.

1. Download the [latest release](https://github.com/shepdio/shepd-dns/releases/tag/v0.0.2)

2. Install on your system with `dpkg -i shepd-dns_<version>.deb`

3. Create a config file with your device token at `/etc/shepd/shepd.conf` (the [SHEPD CLI](https://github.com/shepd-cli) can create this for you automagically)

4. Start the server with `shepd-dns-resolver-client` to listen on port 53. Use `-dns.port=<port>` to specify a different port if, for example, you're not using root or are in a container.

**This software is ALPHA stage and is not yet ready for production use. If you want to help testing, drop us a note at support [at] shepd.io or file an issue on this repository.**
