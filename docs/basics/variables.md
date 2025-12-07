# Variables

A variable is a storage location identified by a name (or identifier) that holds a value. This value can change (or vary) during a program's execution. This is why it's called a variable.

There are two primary ways to create a variable in Go, explicit declaration and shorthand declaration.

## Explicit declaration

```go
package main
import "fmt"
funct main() {
    var age int = 30
    var weight float64 = 70.0
    var name str = "Luis"
    fmt.Println(name, age, weight) # Luis, 30, 70.0
}
```

The var keyword and data type can also be used without having an initial value:

```go
package main
import "fmt"
func main() {
    var age int
    var name string
    var weight float64
    age = 30
    name = "Luis"
    weight = 70.0
    fmt.Println(age, name, weight)
}
```

## Shorthand Variable Declaration
The shorthand variable declaration syntax (```:=```) is a more concise way to declare variables. This method allows you to declare and initialize a variable in a single line without explicitly stating its type, as the type is inferred from the value assigned.

```go
package main
import "fmt"
func main() {
    age := 30
    name := "Luis"
    weight := 70.0
    fmt.Println(age, name, weight)
}
```

## Naming Conventions
- **Use descriptive names**: Use names that clearly describe the purpose or context of the variable.
- **Use CamelCase for Multi-Word Names**: The first word is lowercase, and the first letter of each subsequent word is capitalized.
- **Avoid using Underscore**: Go prefers camelCase over using underscores to separate words in variable names.
- **Use Short Names for Short-Lived Variables**: For short-lived variables, such as loop counters or indices, it's acceptable to use short names like i, j, or k.