# bigcamel

## 用法

```go
package main

import (
    "fmt"

    "github.com/shuguocloud/bigcamel"
)

// out
// Change hello_world to HelloWorld
// Change HelloWorld to hello_world
// Change hello_world_api to HelloWorldAPI

func main() {
    const s string = "hello_world"
    fmt.Printf("Change %s to %s", s, bigcamel.Marshal(s))

    const s1 string = "HelloWorld"
    fmt.Printf("Change %s to %s", s1, bigcamel.UnMarshal(s1))

    const s2 string = "hello_world_api"
    fmt.Printf("Change %s to %s", s2, bigcamel.Marshal(s2))
}
```

### 特点

```
1. 下划线转大驼峰格式（解析）
2. 大驼峰转下划线格式（反解析）
3. 特殊字符不转义

```

