# nihonshufyi

[![Go Reference](https://pkg.go.dev/badge/github.com/fyipedia/nihonshufyi-go.svg)](https://pkg.go.dev/github.com/fyipedia/nihonshufyi-go)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

Sake guide with rice varieties, breweries, and tasting notes — API client for [nihonshufyi.com](https://nihonshufyi.com).

> **Try the interactive tools at [nihonshufyi.com](https://nihonshufyi.com)**

## Install

`go get github.com/fyipedia/nihonshufyi-go`

## Quick Start

```go
package main

import (
    "fmt"
    "fyipedia/nihonshufyi-go"
)

func main() {
    client := nihonshufyi.NewClient()
    result, err := client.Search("dassai-23")
    if err != nil {
        panic(err)
    }
    fmt.Println(result.Total, "results")
}
```

## Also Available

| Platform | Package | Link |
|----------|---------|------|
| **Python** | `pip install nihonshufyi` | [PyPI](https://pypi.org/project/nihonshufyi/) |
| **npm** | `npm install nihonshufyi` | [npm](https://www.npmjs.com/package/nihonshufyi) |
| **Go** | `go get github.com/fyipedia/nihonshufyi-go` | [pkg.go.dev](https://pkg.go.dev/github.com/fyipedia/nihonshufyi-go) |
| **Rust** | `cargo add nihonshufyi` | [crates.io](https://crates.io/crates/nihonshufyi) |
| **Ruby** | `gem install nihonshufyi` | [rubygems](https://rubygems.org/gems/nihonshufyi) |

## Embed Widget

Embed [NihonshuFYI](https://nihonshufyi.com) widgets on any website with [nihonshufyi-embed](https://widget.nihonshufyi.com):

```html
<script src="https://cdn.jsdelivr.net/npm/nihonshufyi-embed@1/dist/embed.min.js"></script>
<div data-nihonshufyi="entity" data-slug="dassai-23"></div>
```

Zero dependencies · Shadow DOM · 4 themes (light/dark/sepia/auto) · [Widget docs](https://widget.nihonshufyi.com)

## Links

- [NihonshuFYI](https://nihonshufyi.com) — Main site
- [API Documentation](https://nihonshufyi.com/developers/)
- [OpenAPI Spec](https://nihonshufyi.com/api/openapi.json)
- [Glossary](https://nihonshufyi.com/glossary/)

## License

MIT
