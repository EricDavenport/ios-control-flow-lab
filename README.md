# Control Flow Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1

What will be printed when the code below is run?  Select all that apply.

```swift
let conditionOne = !(4 < 5) || !(3 > 8)
let conditionTwo = !(!true)

if conditionOne {
 print("A")
} else if conditionTwo {
 print("B")
}
if conditionTwo {
 print("C")
}
print("D")
```

- A
- B
- C
- D

Answer - 
A\n C\n D\n
B will not print because conditionOne renders true before the else statement.

***
## Question 2

What will the code block below print?  Select all that apply:

```swift
let appInfo = (name: "myCoolApp", version: 0.4)
switch appInfo {
 case (_, 0.0..<1.0):
 print("\(appInfo.0) hasn't released yet")
 case ("myCoolApp", _):
 print("Thanks for looking at myCoolApp!")
 default:
 print("I'm not quite sure what you are looking at")
}
```
Answer - 
This should print
"myCoolApp hasn't released yet"

- appInfo.0 hasn't released yet
- myCoolApp hasn't released yet
- Thanks for looking at myCoolApp!
- I'm not quite sure what you are looking at
- It will give a compile-time error

***
## Question 3

What will be printed to the console when the code below is run?  Select all that apply.

```swift
let x: Int = 4
switch x {
case 0..<4:
 print("A")
case 5..<10:
 print("B")
case is Double:
 print("C")
default:
 print("D")
}
```

- A
- B
- C
- D[x] - Answer

***
## Question 4

What are the errors in the code below for the switch statement? Select all that apply.

```swift
let candyType : String = "skittles"

switch candyType {
case "mAndM":
 print("Melts in your mouth, not in your hand")
case "skittles":
 print("Taste the rainbow")
case "snickers":
 print("Hungry? Grab a Snickers")
}


```
Answer
1. There s no default case
1. No additional errors found

- No parentheses around the conditions
- No opening and closing brackets in each of the cases
- No default case in the switch statement
- No print statement right outside the switch statement

***
## Question 5

Given the current weather conditions (rain, sunny, snow), use a switch statement to print an appropriate message to the user

```swift
let currentWeather = "rain"

// enter code below
```
Answer - 
let currentWeather = "rain"

switch currentWeather {
case "rain":
    print("Current weather is rainy, bring an umbrella.")
case "snow":
    print("Current wather is snowy. Bundle up.")
default:  //Sunny
    print("It is pretty nice out. Dress accordingly.")

***
## Question 6

Given the first name and last name of a Fellow, declare `fullName` variable and use string interpolation to concatenate the Fellow's full name and print to the console e.g The Fellow's full name is John Appleseed

```swift
let firstName = "John"
let lastName = "Appleseed"

// enter code below
```
Answer
let firstName = "John"
let lastName = "Appleseed"

print("Fellow's full name is \(firstName) \(lastName)")

***

## Question 7

Convert the if/else statement below into a switch statement.

```swift
if temperatureInFahrenheit <= 40 {
 print("It's cold out.")
} else if temperatureInFahrenheit >= 85 {
 print("It's really warm.")
} else {
 print("Weather is moderate.")
}

//Re-written statement here

```
Answer - 
var temperatureInFarenheit = 86

switch temperatureInFarenheit {
case ..<40:
    print("It's cold out.")
case 85...:
    print("It's really warm.")
default:
    print("Weather is moderate.")
}

***

## Question 8

Complete the following code so that "You win!" is printed.

```swift
if {
 print("You win!")
} 
else {
 print("You lose!")
}
```

let winner = Bool.random()

if winner {
 print("You win!")
}
else {
 print("You lose!")
}
***

## Question 9

Given a variable called numberOfSides, write code using a switch so that it prints out the name of the shape. Account for shapes with 3 to 10 sides and print an error message if out of range.

var numberOfSides = 6

```swift
Example 1:

Input:
var numberOfSides = 4

Output:
Square

Example 2:

Input:
var numberOfSides = 2

Output:
Error

```

var numberOFSides = Int.random(in: 1...10)

switch numberOFSides {
case 3:
    print("\(numberOFSides) sides, Triangle")
case 4:
    print("\(numberOFSides) sides, Square or Rectangle")
case 5:
    print("\(numberOFSides) sides, Pentagon")
case 6:
    print("\(numberOFSides) sides, Hexagon")
case 7:
    print("\(numberOFSides) sides, Heptagon")
case 8:
    print("\(numberOFSides) sides, Octagon")
case 9:
    print("\(numberOFSides) sides, Nonagon")
case 10:
    print("\(numberOFSides) sides, Decagon")
default:
    print("\(numberOFSides) sides, Not a 3 or more sides shape.")
}
***

## Question 10

Create a switch statement that will convert a number grade into a letter grade as shown below:

```swift
Numeric Score 	Letter Grade
100 	A+
90 - 99	A
80 - 89	B
70 - 79 	C
65 - 69 	D
Below 65 	F
```
var myGrade = Int.random(in: 0...100)

switch myGrade {
case 100...:
    print("Number grade is \(myGrade), letter grade is A+")
case 90...99:
    print("Current nuber grande is \(myGrade), A.")
case 80...89:
    print("Current nuber grande is \(myGrade), B.")
case 70...79:
    print("Current nuber grande is \(myGrade), C.")
case 65...69:
    print("Current nuber grande is \(myGrade), D.")
default:
    print("Current grade below passing. \(myGrade).")
}


***

## Question 11

What is wrong with the block of code below?  Correct it so it behaves as expected.

```swift
let firstName = "Peter"

if firstName == "Peter" {
 let lastName = "Gabriel"
} else if firstName == "Phil" {
 let lastName = "Collins"
}
let fullName = firstName + " " + lastName
```
***

## Question 12

Write an if statement that prints out what decade of life someone is in (e.g "You are in your twenties). Then, write it as a switch statement.

```swift
let nameAndBirthYear: (String, Int)

```
***


## Question 13

Consider the below switch statement. What should your system currently print?

```swift
let number = 42

switch number {
case 365:
 print("Days in year")
case 1024:
 print("Bytes in a Kilobyte")
case 0:
 print("Where arrays start")
case 42:
 print("The answer to life, the universe and everything")
default:
 print("Some uninteresting number")
```
Answer - 
System should print, "The answer to life, the universe and everything"
"
What happens when you change number to:
-a. 365?
Days in a year
-b. 1024?
Bytes in a Kilobyte
-c. 65?
"Some uninteresting number"
What happens when you remove the default clause?
"Switch must be exhaustive, do you want to add a default clause"



***


## Question 14

Consider the variable below called population and the if-condition.

a. Add an else-if-condition that states if population is less than 10000 but greater than 5000, then message changes to say it's "a medium size town".

b. Add an else-condition where message changes to say it's a mid-size town.

c. Convert your final if-else statement to a switch statement.

```swift
var population: Int = 10000
var message = String()

if population > 10000 {
 message = "\(population) is a large town"
}
```
var population: Int = 10000
var message = String()

if population >= 10000 {
 message = "\(population) is a large town"
} else if population > 5000 {
    print("This is a meduim sized town.")
} else {
    print("This is a mid-sized town.")
}

***

## Question 15

Complete the code below so that it prints out and tells the user if the sum of the two numbers in the tuple is at least 15.

a. Using a conditional

b. Using a switch statement


```swift
let myTuple: (Int, Int) = (5, 10)
```
Answer - 
a.
if tupleSum == 15{
    print("Sum of both numbers is 15.")
} else {
    print("The sum of the two numbers is \(tupleSum)")
} 

b.
let myTuple: (Int, Int) = (10, 10)
var tupleSum = myTuple.0 + myTuple.1
print(tupleSum)

switch tupleSum {
case 15:
    print("Sum of both numbers is 15.")
default:
    print("The sum of the two numbers is \(tupleSum)")
}
***
