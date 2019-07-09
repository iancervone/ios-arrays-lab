# Arrays lab

Fork and clone this repo. On your fork, answer and commit the follow questions. When you are finished, submit the link to your repo on Canvas.

## Question 1

Create an array of strings called `colors` that contain "orange", "red", "yellow", "turquoise", and "lavender".

Then, using array subscripting and string interpolation, print out the String `"orange, yellow, and lavender are some of my favorite colors"`.

var colors = ["orange", "red", "yellow", "turquoise", "lavender"]

print("\(colors[0]), \(colors[2]), and \(colors[4]) are some of my favorite colors")






## Question 2

Remove "Illinois" and "Kansas" from the array below.

`var westernStates = ["California", "Oregon", "Washington", "Idaho", "Illinois", "Kansas"]`


var westernStates = ["California", "Oregon", "Washington", "Idaho", "Illinois", "Kansas"]
westernStates.removeLast()
westernStates.remove(at: 4)

print(westernStates)




## Question 3

Iterate through the array below. For each state, print out the name of the state, a colon, and whether it is or is not **in the continental United States.**

`let moreStates = ["Hawaii", "New Mexico", "Alaska", "Montana", "Texas", "New York", "Florida"]`



let moreStates = ["Hawaii", "New Mexico", "Alaska", "Montana", "Texas", "New York", "Florida"]
var strangerStates = ["Hawaii", "Alaska"]

for _ in moreStates {
if strangerStates != moreStates {
print("\(moreStates) : is in the continential US")
} else if
strangerStates == moreStates {
print("\(strangerStates) : is not in continential US")
}
}



## Question 4

Print out how many non-whitespace characters are in `myString`:

`let myString = "This is good practice with Strings!"`

Iterate through the array below. For each sentence, print out how many non-whitespace characters are in it.

`let myFavoriteQuotes = ["To be or not to be, that is the question.", "The only source of knowledge is experience.", "Mr. Gorbachev, tear down this wall!", "Four score and twenty years ago..."]`



let myString = "This is good practice with Strings!"
let spaces = myString.components(separatedBy:" ")

var nonWhiteSpace = (myString.count) - (spaces.count-1)
print(nonWhiteSpace)



let myFavoriteQuotes = ["To be or not to be, that is the question.", "The only source of knowledge is experience.", "Mr. Gorbachev, tear down this wall!", "Four score and twenty years ago..."]

let sentence0 = myFavoriteQuotes[0]
let spaces0 = sentence0.components(separatedBy: " ")
print(sentence0.count - spaces0.count-1)

let sentence1 = myFavoriteQuotes[1]
let spaces1 = sentence1.components(separatedBy: " ")
print(sentence1.count - spaces1.count-1)

let sentence2 = myFavoriteQuotes[2]
let spaces2 = sentence2.components(separatedBy: " ")
print(sentence2.count - spaces2.count-1)

let sentence3 = myFavoriteQuotes[3]
let spaces3 = sentence3.components(separatedBy: " ")
print(sentence3.count - spaces3.count-1)





## Question 5

Iterate through `garden` and place any 🌷 that you find into the `basket`. Replace any 🌷 that you pick up with `"dirt"`. Then print how many 🌷 are in your `basket`.

```swift
var garden = ["dirt","🌷","dirt","🌷","dirt","dirt","🌷","dirt","🌷","dirt"]
var basket = [String]()
```


var garden = ["dirt","🌷","dirt","🌷","dirt","dirt","🌷","dirt","🌷","dirt"]
var basket = [String]()

for flowers in garden {
if garden == 🌷{
basket += 1
}
}





## Question 6

The below array represents an unfinished batting lineup for a baseball team. **You, the coach,** need to make some last minute changes:

- Add "Suzuki" to the end of your lineup.
- Change "Jeter" to "Tejada".
- Change "Thomas" for "Guerrero"
- Put "Reyes" to bat 8th instead.

`var battingLineup = ["Reyes", "Jeter", "Ramirez", "Pujols","Griffey","Thomas","Jones", "Rodriguez"]`




var battingLineup = ["Reyes", "Jeter", "Ramirez", "Pujols","Griffey","Thomas","Jones", "Rodriguez"]
battingLineup.append("Suzuki")

if let i = battingLineup.firstIndex(of: "Jeter") {
battingLineup[i] = "Tejada"
}
if let x = battingLineup.firstIndex(of: "Thomas") {
battingLineup[x] = "Guerrero"
}
battingLineup.insert("Reyes", at: 7)

print(battingLineup)





## Question 7

Given an array of Ints, find out if it contains a target number.  

(The built-in `contains(_:)` function will do this, but you aren't allowed to use it for this exercise.)


```swift
var numbers: [Int]

let target: Int = 32
```

Ex.1

```swift
numbers = [4,2,6,73,32,4,2,1]

target = 32

//true
```

Ex. 2

```swift
numbers = [32459,2,4,5,1,4,2,1]

target = 3

//false
```






## Question 8

Find the largest value in an array of Int.  Do not use the built-in `max()` method.

```swift
let arrayOfNumbers: [Int] = (1...100).map{ _ in Int.random(in: 0...200)}.map{Int($0)}

//This creates an array of 100 numbers in between 0 and 200.  For now, you don't need to worry about how it does that.
```


let arrayOfNumbers: [Int] = (1...100).map{ _ in Int.random(in: 0...200)}.map{Int($0)}

var max: Int = 0

for i in arrayOfNumbers {
if i > max {
max = i
}
}
print(max)




## Question 9

Find the smallest value in an array of Int.  Do not use the built in min() method.

```swift
let arrayOfNumbers: [Int] = (1...100).map{ _ in Int.random(in: 0...200)}.map{Int($0)}

//This creates an array of 100 numbers in between 0 and 200.  For now, you don't need to worry about how it does that.
```



let arrayOfNumbers: [Int] = (1...100).map{ _ in Int.random(in: 0...200)}.map{Int($0)}

var min: Int = 200

for i in arrayOfNumbers {
if i < min {
min = i
}
}

print(min)




## Question 10

Iterate through `secondListOfNumbers`, and print out all the odd numbers.

`var secondListOfNumbers = [19,13,14,19,101,10000,141,404]`


var secondListOfNumbers = [19,13,14,19,101,10000,141,404]

for i in secondListOfNumbers {
if i % 2 != 0 {
print(i)
}
}



## Question 11

Iterate through `thirdListOfNumbers`, and print out the sum.

`var thirdListOfNumbers = [11, 26, 49, 61, 25, 40, 74, 3, 22, 23]`

var thirdListOfNumbers = [11, 26, 49, 61, 25, 40, 74, 3, 22, 23]
var sum: Int = 0
for i in thirdListOfNumbers {
sum = sum + i
}
print(sum)



## Question 12

Iterate through `thirdListOfNumbers`, and print out the sum of all the even numbers.

`var thirdListOfNumbers = [11, 26, 49, 61, 25, 40, 74, 3, 22, 23]`



var thirdListOfNumbers = [11, 26, 49, 61, 25, 40, 74, 3, 22, 23]
var evenSum = 0
for i in thirdListOfNumbers {
if i % 2 == 0 {
evenSum = evenSum + i
}
}
print(evenSum)



## Question 13

Append every Int that appears in both `listOne` and `listTwo` to the `sharedElements` array. Then print **how many Ints** are shared.

```swift
var listOne = [28, 64, 7, 96, 13, 32, 94, 11, 80, 68]
var listTwo = [18, 94, 48, 6, 42, 68, 79, 76, 13, 7]
var sharedElements = [Int]()
```

var listOne = [28, 64, 7, 96, 13, 32, 94, 11, 80, 68]
var listTwo = [18, 94, 48, 6, 42, 68, 79, 76, 13, 7]
var sharedElements = [Int]()

for num in listOne {
if listTwo.contains(num) {
sharedElements.append(num)
}
}
print(sharedElements.count)




## Question 14

Write code such that `noDupeList` has all the same Ints as `dupeFriendlyList`, but has no more than one of each Int.

```swift
var dupeFriendlyList = [4,2,6,2,2,6,4,9,2,1]
var noDupeList: [Int] = []
```



var dupeFriendlyList = [4,2,6,2,2,6,4,9,2,1]

var noDupeList: [Int] = []

for i in dupeFriendlyList {
if noDupeList.contains(i) {
} else {
noDupeList.append(i)
}
}
print(noDupeList)





## Question 15

Find the second smallest number in an Array of Ints

`let arrayOfNumbers: [Int] = (1...100).map{ _ in Int.random(in: 0...200)}.map{Int($0)}`



let arrayOfNumbers: [Int] = (1...100).map{ _ in Int.random(in: 0...200)}.map{Int($0)}
var smallestNum: Int = 0
var secondSmallestNum: Int = 200

print(arrayOfNumbers)

for num in arrayOfNumbers {
if ((num > smallestNum) && (num < secondSmallestNum)) {
secondSmallestNum = num
}
}
print(secondSmallestNum)



## Question 16

If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.

Find the sum of all the multiples of 3 or 5 below 1000.



let numberArray = Array(1..<1000)
var multiples: [Int] = []

for num in numberArray {
if num % 3 == 0 || num % 5 == 0 {
multiples.append(num)
}
}

var sum = 0
for i in multiples {
sum = i + sum
}

print(sum)





## Question 17

Make an array that contains all elements that appear **more than twice** in `someRepeatsAgain`.

```swift
var someRepeatsAgain = [25,11,30,31,50,28,4,37,13,20,24,38,28,14,44,33,7,43,39,35,36,42,1,40,7,14,23,46,21,39,11,42,12,38,41,48,20,23,29,24,50,41,38,23,11,30,50,13,13,16,10,8,3,43,10,20,28,39,24,36,21,13,40,25,37,39,31,4,46,20,38,2,7,11,11,41,45,9,49,31,38,23,41,16,49,29,14,6,6,11,5,39,13,17,43,1,1,15,25]
```







## Question 18 (each group of 3 numbers equals 10, but i don't know how to seperate them into triplets)

Identify if there are 3 integers that sum to 10 in the following array. If so, print them as a triplet. If there are multiple triplets, print all possible triplets.

`var tripleSumArr = [-20,-14, -8,-5,-3,-2,1,2,3,4,9,15,20,30]`




var tripleSumArr = [-20,-14,-8,-5,-3,-2,1,2,3,4,9,15,20,30]
var triplet: [Int] = []

for num1 in tripleSumArr {
for num2 in tripleSumArr {
for num3 in tripleSumArr {
if num1 + num2 + num3 == 10 {
triplet.append(num1)
triplet.append(num2)
triplet.append(num3)
}
}
}
}

print(triplet)






## Question 19

Given an array of Strings, find the the String with the most "a"s in it.

input: `["apes", "abba", "apple"]`

output: `"abba"`




let arrayOfStrings: [String] = ["apes", "abba", "apple"]

let string0 = arrayOfStrings[0]
var aInString0 = 0

let string1 = arrayOfStrings[1]
var aInString1 = 0

let string2 = arrayOfStrings[2]
var aInString2 = 0


for a in string0 {
if a == "a" {
aInString0 += 1
}
}

for a in string1 {
if a == "a" {
aInString1 += 1
}
}

for a in string0 {
if a == "a" {
aInString2 += 1
}
}

if aInString0 < aInString1 && aInString0 < aInString2 {
print("\(string2) has the most A's")
} else {
if aInString0 < aInString1 && aInString1 > aInString2 {
print("\(string1) has the most A's")
} else {
print("\(string0) has the most A's")
}
}






## Question 20

Given an Array of Arrays of Ints, find the Array of Ints with the largest sum:

Input: `[[2,4,1],[3,0],[9,3]]`

Output: `[9,3]`




let arrayofInt = [[2,4,1],[3,0],[9,3]]

let set0 = arrayofInt[0]
var set0Sum = 0

let set1 = arrayofInt[1]
var set1Sum = 0

let set2 = arrayofInt[2]
var set2Sum = 0


for num in set0 {
if num != 0 {
set0Sum = set0Sum + num
}
}

for num in set1 {
if num != 0 {
set1Sum = set1Sum + num
}
}

for num in set2 {
if num != 0 {
set2Sum = set2Sum + num
}
}

print(set0Sum)
print(set1Sum)
print(set2Sum)

if set2Sum > set1Sum && set2Sum > set0Sum {
print("\(set2) is the biggest sum")
} else
if set0Sum < set1Sum && set1Sum > set2Sum {
print("\(set1) is the biggest sum")
} else {
print("\(set0) is the biggest sum")
}

if set0Sum < set1Sum && set1Sum > set2Sum {
print("\(set1) is the largest sum")
} else {
if set0Sum < set1Sum && set1Sum < set2Sum {
print("\(set2) is the largest sum")
} else {
print("\(set0) is the largest sum")
}
}






## Question 21

Given an Array of Tuples of type `(Int, Int)`, create an array containing all the tuples where the first Int is equal to the second Int.

Input: `[(4,2), (-3,-3), (1,1), (3,9)]`

Output: `[(-3,-3), (1,1)]`



let tupleArray = [(4,2), (-3,-3), (1,1), (3,9)]

let ta0 = tupleArray[0]
let ta1 = tupleArray[1]
let ta2 = tupleArray[2]
let ta3 = tupleArray[3]

if ta0.0 == ta0.1 {
print(ta1)
}
if ta1.0 == ta1.1 {
print(ta1)
}
if ta2.0 == ta2.1 {
print(ta2)
}
if ta3.0 == ta3.1 {
print(ta3)
}




## Question 22

Given an Array of Bools, make a variable called `allAreTrue` that is true if all of the Bools are true and false if any of them are false.

Input: `[true, false, true, true]`

Output: `false`



let boolArray = [true, false, true, true]
var allAreTrue: Bool?

for truth in boolArray {
if truth != true {
allAreTrue = false
break
} else {
allAreTrue = true
}
}

print(allAreTrue!)





## Question 23

Given an Array of Ranges of Ints, create an array that has all the values from all the ranges in order from smallest to greatest with no duplicates.

Input: `[0..<3 , 2..<10, -4..<6, 13..<14]`

Output: `[-4,-3,-2,-1,0,1,2,3,4,5,6,7,8,9,10,13]`


## Question 24

Given an array of Characters, create a String ignoring and uppercase Characters and spaces.  Then uppercase every other character of the String.

Input: `let arr: [Character] = ["a", "p","P","l","E"," ","S","a","u","C,"e"]`

Output: `"ApLeAuE"`


## Question 25

Print out each element in `myMatrix`

`var myMatrix = [[10, 14, 12], [91, 1, 9], [31, 3, 21]]`


var myMatrix = [[10, 14, 12], [91, 1, 9], [31, 3, 21]]

for (arrayIndex, arrayElement) in myMatrix.enumerated() {
for (elementIndex, elementInt) in arrayElement.enumerated() {
print(elementInt)

}
}


## Question 26

Print out the sum of the diagonals of `myMatrix`.

`var myMatrix = [[10, 14, 12], [91, 1, 9], [31, 3, 21]]`



var myMatrix = [[10, 14, 12], [91, 1, 9], [31, 3, 21]]
var diagonalSum = 0


for (arrayIndex, arrayElement) in myMatrix.enumerated() {
for (elementIndex, elementInt) in arrayElement.enumerated() {
if arrayIndex == elementIndex {
diagonalSum = diagonalSum + elementInt

}
if arrayIndex + elementIndex == myMatrix.count - 1 {
diagonalSum = diagonalSum + elementInt
}
}
}
print(diagonalSum)




## Question 27

Using for loops, rotate `matrixToRotate` 90 degrees.

var matrixToRotate = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]

![Matrix Rotation](images/rotated_matrix.jpeg)


