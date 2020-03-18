# Outputting text in Kotlin

## Extending Hello World

In the previous topic, the anatomy of `Hello World` was broken down. The code will now be extended with a variant of the `println()` function named `print()`:

``` kotlin
 fun main() {
     println("hello")
     print("my name is")
     print("thomas")

     println("This version will properly end in a newline")
     print("I can also print a number: ")
     print(5)
     println(", and notice how the number didn't need quotes")
 }
```

Output:
```
hello
my name isthomasThis version will properly end in a newline
I can also print numbers: 5, and notice how the number didn't need quotes
```

Notice there is some unintended side effects.

## print() vs println()

After `println()` is finished printing its argument, it will print a special **newline** character. This results in the next instance of printing to the screen to be on the line below.

#### Example using println()
``` kotlin
fun main() {
  println("hello")
  println("goodbye")
}
```
Output:
```
hello
goodbye
```

The second line, printing "goodbye", appears on a second line per the usage of `println()` in the first line.

On the other hand, using `print()` instead will **not** add a newline after the print statement:

### Example using print()
``` kotlin
fun main() {
  print("hello")
  print("goodbye")
}
```
Output:
```
hellogoodbye
```
As there was no `newline`, it appears in one line, or as one continuing word.

## Printing Numbers

Se are not limited to printing quotes of text. We can also print numbers just fine. This serves a short introduction to the next topic.

### Example
``` kotlin
fun main() {
  print(5)
  print(" is my favorite number")
}
```
Output:
```
5 is my favorite number
```
Take note of the intended blank character in the quote `" is my favorite character"`. This allows the output to have a space and can be read as a proper sentence.

## Practice Problems

*Write code that will print the following text. All numbers **must** be a true number, not part of a quote.*

1. ``` 
Hello
Today is Thursday, the 5th
```
2. ```
Number of passengers: 6
Number of seats: 5
```
3. ```
5 4 2
6 2 4
```


## Closing notes

Being familiar with the nuances of printing to the screen will be critical going forward as the near entirety of this course will involve printing information to the terminal. It is essential to understand this topic despite it being rather dull.

---


 - **Next Topic**: [02. Variables, Input, Arithmetic](2_variables_input_arithmetic.md)
 - **Prev Topic**: [00. Getting Started](0_getting_started.md)


 - **Jump Back** to [Course Outline](README.md).
