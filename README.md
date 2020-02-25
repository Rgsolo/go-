#### 库源码文件和命令源码文件

```go
package main

import (
  "flag"
)

var name string

func init() {
  flag.StringVar(&name, "name", "everyone", "The greeting object.")
}

func main() {
  flag.Parse()
  hello(name)
}
```

