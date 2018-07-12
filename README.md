# google-go (golang)
Manual and shortcuts. More information in:  
https://golang.org/doc/code.html

It is a good practice to create a project inside your "github" account to prevent package collisions:

```bash
mkdir -p $GOPATH/src/github.com/gchumillas
```

creates a go file

```go
package main

import "fmt"

func main() {
	fmt.Printf("Hello, world.\n")
}
```

and install it

```bash
# this command can be executed from anywhere
go install github.com/user/hello
```

The previous command creates an executable into the `$GOPATH/bin` folder.

**More useful instructions:**
```bash
# Install and alternatively update (-u) a package dependency
go -u github.com/path/to/package
```
