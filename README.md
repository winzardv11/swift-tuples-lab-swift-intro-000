# Tuples Lab

<img src="http://viaimmobiler.com/wp-content/uploads/2016/05/john-candy-planes-trains-and-automobiles-del.jpg" alt="Drawing" style="width: 200px;"/>  


> Whoever said nothing is impossible obviously hasn't tried nailing Jell-O to a tree.

 

## Learning Objectives - The student should be able to..

* Answer the questions in this lab and be challenged on their knowledge of tuples.

## What the student can do at this point 

* Create variables and constants
* Is familiar with type annotations, type inference and string interpolation.
* Can create functions with return types.
* Is familiar with the String, Int, Double, and Bool type.
* Can perform arithmetic operations on Int and Double.
* Understands if and else clause statements.
* Can create and use Arrays.
* Can iterate over an Array using a for-in loop.
* Can iterate over an Array calling enumerate().
* Work with the following methods on arrays:
	* append()
	* insert(_:atIndex:)
	* removeAtIndex()
	* subscript syntax with arrays
	* count
	* isEmpty
	* Optionals
* Just learned about Tuples

## Outline / Notes

*  This could be anywhere between 10-15 questions.
*  One of the questions towards the end can ask them to produce something like the following: Create a function that takes in an array of Int's and the function needs to return back the min and max in a tuple.

```swift
func minMaxFromArray(array: [Int]) -> (min: Int, max: Int) {
    
    var min = array[0]
    var max = array[0]
    
    for number in array {
        if number < min { min = number }
        if number > max { max = number }
    }
    
    return (min, max)
}
```

* Another question could have them answer something like the following. I like the idea of encouraging them to try solving this problem with a switch statement:

```swift
func numberOfOnesAndTwosFromNumbers(numbers: [Int]) -> (ones: Int, twos: Int) {
    
    var numberOfOnes = 0
    var numberOfTwos = 0
    
    for number in numbers {

        switch number {
        case 1: numberOfOnes += 1
        case 2: numberOfTwos += 1
        default: break
        }
        
    }
    
    return (numberOfOnes, numberOfTwos)
}
```




<a href='https://learn.co/lessons/TuplesLab' data-visibility='hidden'>View this lesson on Learn.co</a>
