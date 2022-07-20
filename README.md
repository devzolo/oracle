# GORM Oracle Driver

## Required dependency Install

- Oracle 12C+
- Golang 1.13+
- see [ODPI-C Installation.](https://oracle.github.io/odpi/doc/installation.html)

## Quick Start

### how to install

```bash
go get github.com/devzolo/oracle
```

### usage

```go
import (
 "fmt"
 "github.com/devzolo/oracle"
 "gorm.io/gorm"
 "log"
)

func main() {
    db, err := gorm.Open(oracle.Open("system/oracle@127.0.0.1:1521/XE"), &gorm.Config{})
    if err != nil {
        // panic error or log error info
    }

    // do somethings
}
```
