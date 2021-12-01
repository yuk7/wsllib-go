# wsllib-go
A WSL Library for Golang.

## Usage
Get this package
```
go get github.com/yuk7/wsllib-go
```

## Example
```go
package main

import "github.com/yuk7/wsllib-go"

func main() {
    wsllib.WslLaunchInteractive("DistroName", "", true)
}
```

## Notes
WslLaunchInteractive is not used in this library as it causes problems in goroutine.

Instead, a function is defined to connect stdin, stdout, stderr to WslLaunch.
