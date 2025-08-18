# Whois

Whois is a release tool for domain and ip whois information query.

## Overview

All of domain, IP include IPv4 and IPv6, ASN are supported.

**This is a fork of [github.com/likexian/whois](https://github.com/likexian/whois) maintained by Mailgun.**

## Usage

### whois query for domain

```shell
whois example.com
```

### whois query for IPv6

```shell
whois 2001:dc7::1
```

### whois query for IPv4

```shell
whois 1.1.1.1
```

### whois query for ASN

```shell
# or whois as60614
whois 60614
```

### whois query output as json

```shell
whois -j example.com
```

## License

Copyright 2014-2024 [Li Kexian](https://www.likexian.com/)
Copyright 2019-2025 Mailgun Technologies, Inc.

Licensed under the Apache License 2.0

## Donation

If this project is helpful, please share it with friends.

If you want to thank the original author, you can [give Li Kexian a cup of coffee](https://www.likexian.com/donate/).
