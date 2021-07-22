# Arrary 101 note
[Original Website](https://leetcode.com/explore/learn/card/fun-with-arrays/)

# Overview
After completing this Explore Card on Arrays, you will understand:
- what an array is
- basic properties of arrays
- implementing basic array operations
- simple programming techniques with arrays

# Introduction
## What is an array
we'll start by comparing arrays to a real-world problem: storing lots of DVDs in an organized way. 
> An array is a collection of items. The items could be integers, strings, DVDs, games, books. The items are stored 
> in neighboring (contiguous) memory locations. Because they're stored together, checking through the entire 
> collection of items is straightforward. 

In **Java**, we using following code to create an array to hold up to 15 DVDs.

```java 
// The actual code for creating an Array to hold DVD's.
DVD[] dvdCollection = new DVD[15];

// A simple definition for a DVD.
public class DVD {
    public String name;
    public int releaseYear;
    public String director;

    public DVD(String name, int releaseYear, String director) {
        this.name = name;
        this.releaseYear = releaseYear;
        this.director = director;
    }

    public String toString() {
        System.out.println(
            this.name + ", directed by " + this.director + ", released in " + this.releaseYear));
    }
}
```
## Array capacity VS Length
1. Capacity: number of DVDs the box could hold, if it was full
2. Length: number of DVDs currently in the box 
Trying to put an element beyonds its capacity will cause your code to crash with an ```
ArrayIndexOutOfBoundsException``` Array's capacity must be decided when array is created. Then capacity
can't be changed later. 
```java
// Create a new array with a capacity of 6.
int[] array = new int[6];

// Current length is 0, because it has 0 elements.
int length = 0;

// Add 3 items into it.
for (int i = 0; i < 3; i++) {
    array[i] = i * i;
    // Each time we add an element, the length goes up by one.
    length++;
}

System.out.println("The Array has a capacity of " + array.length);
System.out.println("The Array has a length of " + length);
```
output will be like:
```The Array has a capacity of 6. The Array has a length of 3```

Exerciese 1: Given a binary array nums, return the maximum number of consecutive 1's in the array.(solution in python)
```python
class Solution(object):
    def findMaxConsecutiveOnes(self, nums):
        """
        :type nums: List[int]
        :rtype: int
        """
        max_result = 0
        temp = 0
        for i in nums:
            if i == 1:
                temp = temp + 1 
            else:
                if temp > max_result:
                    max_result = temp
                temp = 0
        if temp > max_result:
            max_result = temp
                
        return max_result
```
# Inserting Items Into an Array

# Deleting Items From an Array

# Searching for Items in an Array

# In-Place Operations

# Conclusion

# English Note
- being a guru with something: 领导，指导，完全理解
- consecutive 连续的
