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
## Accessing elements in arrays


# Inserting Items Into an Array

# Deleting Items From an Array

# Searching for Items in an Array

# In-Place Operations

# Conclusion

# English Note
- being a guru with something: 领导，指导，完全理解
