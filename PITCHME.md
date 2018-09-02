# @color[#DC322F](Scala)
## In multiple Nutshells

---
@snap[north-west]

### What is @color[#DC322F](Scala)?

@ul 

- Scala combines object-oriented and functional programming in one concise, high-level language. 
- Scala stands for "Scalable Language"
- Strongly Typed (everything is an object)

@ulend

+++
@snap[north-west]

### But wait, there is more!

@ul

- The Community
- Libraries
- Cross-Platform
- Cross-Backend
- Sugar

@ulend

+++
@snap[north-west]

### Who uses @color[#DC322F](scala)?

@ul

- Twitter
- Zalando
- IBM
- SAP
- Moia
- LinkedIn
- Netflix
- Verizon

@ulend

+++
@snap[north-west]

### Why @color[#DC322F](scala)?

@ul

- Flexible
- Dynamic
- Safe
- Efficient
- Scalable
- Predictable

@ulend

+++
@snap[north-west]

### Where is @color[#DC322F](scala) used?

@ul

 - Traditional Full Stack
 - Web API endpoints
 - Data Analysis & Big Data
 - Data Streaming
 - Front end (scala.js)
 - Neural Networks
 - Natural Language Processing
 - Native Code (scala-native)

@ulend

---

## Setup

+++
@snap[north-west]

### Installation  

<br><br>

#### Linux...  
##### It is complicated  

<br>

#### MacOS  
`brew install sbt`

<br>

#### Windows...  
##### IntelliJ  

+++

### A Solution!

@snap[north-west]

#### scastie! 
scastie.scala-lang.org

#### scalafiddle
scalafiddle.io

---

### Basics

+++

### REPL

```scala

scala> 2 + 2
res0: Int = 4

scala> res0 + 2
res1: Int = 6

```

+++

### Hello World

```scala
println("Hello World!")
println(10)

// Hello World!
// 10
```

+++

### Variables

```scala

val x = 10

x = 20 // error: reassignment to val

var y = 10
y = 20

```

+++

### Type Inference & Type Annotations

```scala

val z = 10 // Inferred integer type

val a: Int = 20
val b: Double = 3.0

val c: Double = 40 // Automatic conversion

```

+++

### The Boolean Type

```scala

true
false

!true         // false
!false        // true

true == false // false
10 > 5        // true

```

+++

### Math

```scala

1   + 1   //  2
2   - 1   //  1
5   * 3   // 15
6   / 2   //  3
6   / 4   //  1
6.0 / 4   //  1.5
6   / 4.0 //  1.5
```

+++

### Strings

```scala

"Scala strings are surrounded by quotes"

'a' // A Char

```

+++

### String Operations

```scala

"hello world".length
"hello world".substring(2, 6)
"hello world".replace("C", "3")

```

+++

### Extra String Operations

```scala

"hello world".take(5)
"hello world".drop(5)

```

+++

### String Interpolation

```scala

val apples = 12
s"We have $apples apples" // => "We have 12 apples"

val oranges = 5
s"We have ${apples + oranges} fruit" // => "We have 17 fruit"

```

+++

### More String Interpolation

```scala

f"Square root of 122: ${math.sqrt(122)}%1.4f" // => "Square root of 122: 11.0454"

```

+++

### Tuples

```scala

val foo = ("Hello", true, 100)

val bar = foo._2 // true

val baz: (Int, Double, String) = (1, 2.0, "three")

val qux: (Int, Double) = (1, 2)

```

+++

### Functions

```scala
def sumOfSquares(a: Int, b: Int): Int = {
  val a2 = a * a
  val b2 = b * b
  a2 + b2
}
```

```scala
def sumOfSquares(a: Int, b: Int) = a * a + b * b
```

```scala
sumOfSquares(3, 4) // => 25
```

+++

### Named & Default Parameters

```scala

def greet(name: String, greeting: String = "Hello") {
  println(greeting + " " + name)
}

greet("Florian")     // Hello Florian
greet("Andre", "Hi") // Hi Andre
greet(greeting = "Wazzup", "Tim") // Wazzup Tim

```

+++

### Multiple Return Values

```scala

def addAndSub(a: Int, b: Int): (Int, Int) = {
  (a + b, a - b)
}

val (foo, bar) = addAndSub(3, 2)
// foo => 5
// bar => 1

```

+++

### Lambdas / Anonymous Functions

```scala

val sq = (x: Int) => x * x

sq(10) // => 100

```

```scala

val sq: Int => Int =
  x => x * x

```

### The Magic Underscore

```scala

val addOne: Int => Int =
  _ + 1

addOne(5) // => 5

```

```scala

val weirdSum: (Int, Int) => Int =
  (_ * 2 + _ * 3)
  
weirdSum(2, 5) // => 19

```









