# Types Variables Logic and Operations Lab 2

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1 DONE

You are given three grades obtained by 3 students, which are stored in variables `grade1`, `grade2`, `grade3` and all of type `Double`.
Create a variable called `yourGrade` of type `Double` and give it a value.
Print `"above average"` if your grade is greater than the class average or `"below average"` otherwise.

```swift
var grade1 = 7.0
var grade2 = 9.0
var grade3 = 5.0

// your code here
```

Answer:
```swift
var grade1 = 7.0
var grade2 = 9.0
var grade3 = 5.0

var myGrade: Double = 10.0

var classAverage = (grade1 + grade2 + grade3 + myGrade)/4

if myGrade > classAverage {
print("above average")
} else {
print("below average")
}
```

***
## Question 2 DONE

You are given a number. Print even if the number is even or odd otherwise.

```swift
let number = 2
// your code here
```

Answer:
```swift
let number = 2

if number % 2 == 0 {
print("even")
} else {
print("odd")
}
```

***
## Question 3 DONE

You are given two numbers `a` and `b`. Print `"divisible"` if `a` is divisible by `b` and `"not divisible"` otherwise.

```swift
var a = 12
var b = 3

// code here
```

Answer:
```swift
var a = 12
var b = 3

if a%b == 0 {
print("divisible")
} else {
print("not divisible")
}
```

***
## Question 4 DONE

You are given three variables `a`, `b` and `c`. Check if at least two variables have the same value. If that is true, print `"At least two variables have the same value"` otherwise print `"All the values are different"`.

```swift
var a = 2
var b = 3
var c = 2

// your code here
```

Answer:
```swift
var a = 2
var b = 3
var c = 2

if a == b || a == c || b == c {
print("At least two variables have the same value")
} else {
print("All the values are different")
}
```

***
## Question 5 DONE

You are working on a smart-fridge. The smart-fridge knows how old the eggs and bacon in it are. You know that eggs spoil after 3 weeks (21 days) and bacon after one week (7 days). Given `baconAge` and `eggsAge` (both in days) determine if you can cook bacon and eggs, or which ingredients you need to throw out. If you can cook bacon and eggs, print `"you can cook bacon and eggs"`. If you need to throw out any ingredients, for each one print a line with the text `"throw out"` + bacon or eggs.

```swift
var baconAge = 6 // the bacon is 6 days old
var eggsAge = 12 // eggs are 12 days old

// your code here
```

Answer:
```swift
var baconAge = 6 // the bacon is 6 days old, spoils after 7 days
var eggsAge = 12 // eggs are 12 days old, spoils after 21 days
var baconExpDays = 7
var eggsExpDays = 21

if baconAge <= 7 && eggsAge <= 21 {
print("you can cook bacon and eggs")
}
if baconAge > baconExpDays {
print("throw out bacon")
}
if eggsAge > eggsExpDays {
print("throw out eggs")
}
```

***
## Question 6 DONE

You are given a year, determine if it’s a leap year. A leap year is a year containing an extra day. It has 366 days instead of the normal 365 days. The extra day is added in February, which has 29 days instead of the normal 28 days. Leap years occur every 4 years. 2012 was a leap year and 2016 will also be a leap year.
The above rule is valid except that every 100 years special rules apply. Years that are divisible by 100 are not leap years if they are not also divisible by 400. For example 1900 was not a leap year, but 2000 was. Print `"Leap year!"` or `"Not a leap year!"` depending on the year you are provided.

```swift
let year = 2014

// your code here
```

Answer:
```swift
let year = 2014
// True if % 400
// False if % 100
// True if % 4

if year % 400 == 0 {
print("Leap year!")
} else if year % 100 == 0 {
print("Not a leap year!")
} else if year % 4 == 0 {
print("Leap year!")
} else {
print("Not a leap year!")
}
```

***
## Question 7 DONE

If you use `random()` it will give you a random number within a specified range. Generate a random number and use it to simulate a coin toss. Print `"heads"` or `"tails"`.

```swift
let randomNum = Int.random(in: 0...100)

// your code here
```

Answer:
```swift
let randomNum = Int.random(in:0...100)
var heads = 51...100

switch randomNum {
case heads:
print("heads")
default:
print("tails")
}

```

Hint: use an if/else block along with the `%` operator

***
## Question 8 DONE

You are given four variables `a`, `b`, `c` and `d`. Print the value of the smallest one.

```swift
var a = 5
var b = 6
var c = 3
var d = 4

// your code here
var a = 5
var b = 6
var c = 3
var d = 4

let smallest = min(a,b,c,d)
print(smallest)
```

***
