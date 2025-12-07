# Basic Data Types in Go

This documentation explains the **basic (primitives-like) data types in go**.

---

## What is a Data Type?
A **data type** defines:
- What kind of value a variable holds
- What operations can be applied to it
- How it behaves in memory

Every value in Go has a type:
```go
package main
import ("fmt" "reflec")
func main() {
    x := 3.4
    t := reflect.TypeOf(x)
    fmt.println("Data type:", x) # Data type : float64

}
```
## Primitives-Like Types in Go
These types represent **single value** and are inmutable.

```int``` - **Integer**

Represent whole numbers (positives, negatives, zero). There are various kinds of integer types associated with int, example:  ```int8```, ```int32```


```go
x := 10
y := -5
z := 0
```
**Features**:
- Fixed Arbitrary size: int is either ```32``` or ```64``` bits depending on architecture. Specific types include ```int8```, ```int16```, etc.
- Overflow is possible if the value exceeds the type's range.
- No automatic type promotion: Operations between ```int``` and ```int64``` for example require explicit converion.
- Supports all standard arithmetric operations

```float``` - **Floating-Point Number**

Represent decimal numbers or in exponential form.

```go
price := 30.5
```
**Important Notes**:
- Fixed precision: Two main types: ```float32``` and ```float64``` (default)
- Supports standard arithmetic operations
- No automatic type promotion

```go
package main

import "fmt"

func main() {
    var a float64 = 3.14
    var b float64 = 2.71

    sum := a + b
    fmt.Println(sum) // 5.85
}
```

```bool``` - **Boolean**

Represent logical truth values.

```go
is_active := True
is_admin := False
```
Used in:
- Conditions.
- Loops.
- Validations.
- Logical operations.

```str``` - **String (Text)**

Used to represent text.

```go
name := "Luis"
message := "Hello world"
```