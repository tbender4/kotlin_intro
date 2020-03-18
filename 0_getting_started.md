# Getting Started with Kotlin

## Getting Started

Kotlin's official Getting Started guide will get you up to speed to compiling `Hello World`. The sidebar can let you choose different setup options. Using **Intellj IDEA** is the recommended setup option. [Please use their resource.](https://kotlinlang.org/docs/tutorials/getting-started.html)

## Hello World Breakdown

The following code is your first Kotlin program: `Hello World`.

```
 fun main() {
     println("hello")
 }
```

This is all that's required to print **hello** in your terminal. This code snippet has components to be mindful of. Let's break down its anatomy:

### The print function and its argument
 ```
 println("hello")
 ```
This line has two components: `println()` is a **function**. A function is a callable command in code that has a specific purpose; and in this case, it will print text to your terminal. There are many built-in functions available in Kotlin and this is the first one to learn.

Any information passed *to the function* is called its **argument(s)** and is placed inside the function's `()` parentheses. In this instance, it has only one argument: A quote of `"Hello"`.

One note about `"hello"`: This is NOT the same as `hello`. The `" "` quotations are required as this is a `string` datatype. Datatypes is an upcoming topic to explain this in more detail.

**In summary**: `println("my text")` is a function that will print anything inside its `()` brackets onto your display.

### The main function
```
fun main() {
}
```
The **main() function** is special type of function that is required for any Kotlin program to run. This is explicitly where your program starts. For now all of your code will be written inside `main()`. Eventually, your code will reside in more than one file and these files will have multiple functions.

Take note to how `main()` is preceded by `fun`, and succeeded by `{`. This is a format requirement that will be taken for granted for now and will be properly explained during the functions topic.

**Any code you wish to run must be inside the `{}` curly brackets.** Code after the ending `}`bracket will not be considered. All code inside this `{}` brackets is considered part of `main()`. Inside the brackets the code will be read in a *top-down* manner. This means every line of code is executed starting from the top of the brackets and goes line-by-line until the end bracket is reached. Code is also read from left to right.

#### Example
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

Notice how `"hello"` was printed before `"goodbye"`. While this may appear obvious, this must be stressed during the next couple of topics.

## Closing notes

If you've made it through this far, good work! Never underestimate your personal progression. As a reminder, do pay attention to anything bold or highlighted as this information will remain relevant.

---

 - Next Topic: [01. Output](1_output.md)
 - Jump Back to [Course Outline](README.md).
