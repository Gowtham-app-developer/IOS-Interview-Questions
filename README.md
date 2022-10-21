# IOS-Interview-Questions
List of top Flutter and Dart Interview Questions &amp; Answers.


## var & let

- Var is mutable (i.e.) Values of the variable can be changed later.
- let is immutable (i.e.) Values of the variable cannot be changed later.

__Example__

```ruby
// TODO Mutable String
var greeting = "Hello, playground"
greeting = "Hello World"
print(greeting)

// TODO Explicitly defining the String
var helloWorld: String
helloWorld = "Hello"
print(helloWorld)

// TODO Immutable Int
let intValue: Int
intValue = 1
print(intValue)
```

## Basics

__Examples__

```ruby
// TODO 1.Variable Declration

// TODO 1.1 Mutable String
var greeting = "Hello, playground"
greeting = "Hello World"
print(greeting)

// TODO 1.2 Explicitly Defining the String
var helloWorld: String
helloWorld = "Hello"
print(helloWorld)

// TODO 1.3 Immutable Int
let intValue: Int
intValue = 1
var intValueTwo = 2

// TODO 2.Operators
print(intValue + intValueTwo)

// TODO 3. Ranges
var values = 1..<5
print(values.contains(5))

// TODO 4.String Interpolation and Concadination

var noOfDays = "30"
var noOfWeek = "4"

print(noOfDays + " " + noOfWeek)
print("No Of Days \(noOfDays)")


// TODO 4.1 Methods in Strings

greeting.contains("p")
greeting.split(separator: ",")
greeting.isEmpty
greeting.count

// TODO 5.Type Conversion

var one = "1"
var two = "2"

var conversionOne = Int(one)
var conversionTwo = Int(two)
var addValues = (conversionOne ?? 0) + (conversionTwo ?? 0)

// TODO 6.Logical Operators

var isLoggedIn: Bool = false
isLoggedIn = !isLoggedIn

var isHavingCard = true
var allowUser = isLoggedIn && isHavingCard
print(allowUser)

// TODO 7.Null Safety Operators

// TODO 7.1 Optionals
var valueOne: String?
var valueTwo: String?

valueOne = "Gauthy"
valueTwo = "Sony"

print(valueOne)

// TODO 7.2 forced unwrapping

print(valueTwo!)

// TODO 7.3 Optional binding

print(valueOne ?? "One")

// TODO 8.Arrays and Methods

var countries: [String] = ["India", "America", "Russia"]
var states: Array<String> = Array<String>()

countries.count
countries.isEmpty
countries.append("China")
countries[0]
countries[0] = "Jai-Hind"
countries
countries.insert("India", at: 0)

countries.sort() // TODO They won't take the copy of the Array
countries.reverse()
countries.sorted() // TODO It Works by taking the copy of the Array
countries.reversed()

// TODO 9.Dictionaries

// TODO Dictionaries - They are key value pairs and are not organized or arranged

var listOfStates: [Int: String] = [
    1: "TamilNadu",
    2: "Kerala",
    3: "Karnataka"
]

var stateValues = listOfStates[1]
listOfStates.keys
listOfStates.values

[Int](listOfStates.keys)
[String](listOfStates.values)

listOfStates.updateValue("Delhi", forKey: 2)
listOfStates

listOfStates[2] = nil // TODO For Removing
listOfStates

listOfStates.removeValue(forKey: 3) // TODO For Removing alternative
listOfStates

var listOfQuestions =
[
    "Question1":[
        "Question":"How are you?",
        "Answer":"fine"
    ],
    "Question2":[
        "Question":"How is your Health?",
        "Answer":"Good"
    ]
]

listOfQuestions["Question1"]?["Answer"]

// TODO 10. Sets

// TODO Sets automatically going to store only the unique Values

// PTR:- In the Sets all the Values should be Hashable

var challengesOne : Set<String> = [
    "One",
    "Two",
    "One",
    "Four"
]

challengesOne

challengesOne.contains("One")
challengesOne.sorted()

var challengesTwo : Set<String> = [
    "Five",
    "Six",
    "One",
    "Two"
]

challengesTwo

// TODO Intersection means common b/w two of these challenges

var intersectionChallenges = challengesOne.intersection(challengesTwo)

// TODO symmetricDifference means the unique values b/w these two

challengesOne.symmetricDifference(challengesTwo)

// TODO 11.Tuples

var course: (String, Int, Bool) = ("Google", 1, true)
course.0

var(company, ID, Status) = course
company

// TODO 11.1 Named Tuples

var courseOne: (companyOne: String, IDTwo: Int, StatusThree: Bool) = ("Google", 1, true)
courseOne.0

var(companyOne, IDTwo, StatusThree) = courseOne
company
```
