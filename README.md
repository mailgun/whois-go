# Whois

[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
[![GoDoc](https://pkg.go.dev/badge/github.com/mailgun/whois-go.svg)](https://pkg.go.dev/github.com/mailgun/whois-go)

**This is a fork of [github.com/likexian/whois](https://github.com/likexian/whois) maintained by Mailgun.**

Whois is a simple Go module for domain and ip whois information query.

## Overview

All of domain, IP include IPv4 and IPv6, ASN are supported.

You can directly using the binary distributions whois, follow [whois release tool](cmd/whois).

Or you can do development by using this golang module as below.

## Installation

```shell
go get -u github.com/mailgun/whois-go
```

## Importing

```go
import (
    "github.com/mailgun/whois-go"
)
```

## Documentation

Visit the docs on [GoDoc](https://pkg.go.dev/github.com/mailgun/whois-go)

## Example

### whois query for domain

```go
result, err := whois.Whois("likexian.com")
if err == nil {
    fmt.Println(result)
}
```

### whois query for IPv6

```go
result, err := whois.Whois("2001:dc7::1")
if err == nil {
    fmt.Println(result)
}
```

### whois query for IPv4

```go
result, err := whois.Whois("1.1.1.1")
if err == nil {
    fmt.Println(result)
}
```

### whois query for ASN

```go
// or whois.Whois("AS60614")
result, err := whois.Whois("60614")
if err == nil {
    fmt.Println(result)
}
```

## Whois information parsing

Please refer to [whois-parser](https://github.com/likexian/whois-parser)

## License

Copyright 2014-2025 [Li Kexian](https://www.likexian.com/)
Copyright 2019-2025 Mailgun Technologies, Inc.

Licensed under the Apache License 2.0

## Donation

If this project is helpful, please share it with friends.

If you want to thank the original author, you can [give Li Kexian a cup of coffee](https://www.likexian.com/donate/).
