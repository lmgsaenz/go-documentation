# Conditionals

## IF statement

if statement evaluates a condition and executes a statement block enclosed in curly braces {..} if the evaluation returns true. The condition may be optionally enclosed inside a pair of parentheses (...).

```go
if sick {
    fmt.Println(Stay at home.)
}
```
```go
if (healthy) {
    fmt.Println(Work.)
}
```

## Else statement

else statement can succeed an if or if else-if statement block and its code executed if the conditions in the preceding if or if else-if statements evaluate to false.
```go
sick := false
if sick {
  fmt.Println("Call the doctor.")
} else {
  fmt.Println("Enjoy your day.")
}
```

## Else If statement
else if statement provides an additional condition to evaluate besides the first if conditional. It can only appear after the if statement and before an else statement if it exists. For example:

```go
if (temperature < 15) {
  fmt.Println("Put on a jacket.")
} else if (temperature >= 15 && temperature < 20) {
  fmt.Println("Put on a light sweater.")
} else {
  fmt.Println("Wear summer clothes.")
}
```
Multiple else if statements can exist alongside the if statement. The if else if statements are scanned from top to bottom and only the code block associated with a true condition is executed. If none of the conditions are satisfied, the else code block is executed if it exists.

## Switch statement
The Go switch statement can be used as an alternative to a set of if followed by else if statements. The switch statement compares the expression inside a condition with a set of values encapsulated in cases. The code inside a matched case value is executed and the switch block terminates. A default case without a value can be appended to the last case and its code executed if no prior match is found.
```go
day := "Tuesday"
switch day {
  case "Monday":
    fmt.Println("Monday is magnificent.")
  case "Tuesday":
    fmt.Println("Tuesday is terrific.")
  case "Wednesday":
    fmt.Println("Wednesday is wacky.")
  default:
    fmt.Println("We survived.")
}
```