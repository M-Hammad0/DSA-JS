# DSA - JS - Revision
Hi! I'm your first Markdown file in **StackEdit**. If you want to learn about StackEdit, you can read me. If you want to play with Markdown, you can edit me. Once you have finished with me, you can create new files by opening the **file explorer** on the left corner of the navigation bar.


# Big O Notation
-   To analyze the performance of an algorithm, we use Big O Notation
-   Big O Notation can give us a high level understanding of the time or space complexity of an algorithm
-   Big O Notation doesn't care about precision, only about general trends (linear? quadratic? constant?)
-   The time or space complexity (as measured by Big O) depends only on the algorithm, not the hardware used to run the algorithm

![image info](./images/t_complexity_graph.png)

> 

## Time Complexity

 **Constants Don't Matter**

```
O(2n) 				O(n)
O(500)				O(1)
O(13n^2)			O(n^2) 
```

**Smaller Terms Don't Matter**
```
O(n+1o)				O(n)
```
**Big O Shorthands**
```
-   Arithmetic operations are constant
-   Variable assignment is constant
-   Accessing elements in an array (by index) or object (by key) is constant
-   In a loop, the the complexity is the length of the loop times the complexity of whatever happens inside of the loop
```

## Space Complexity

```
-   Most primitives (booleans, numbers, undefined, null) are constant space
-   Strings require O(n) space (where n is the string length)
-   Reference types are generally O(n), where n is the length (for arrays) or the number of keys (for objects)
```


# Problem Solving Approach


## UNDERSTAND THE PROBLEM
1.  Can I restate the problem in my own words?
2.  What are the inputs that go into the problem?
3.  What are the outputs that should come from the solution to the problem?
4.  Can the outputs be determined from the inputs? In other words, do I have enough information to solve the problem? (You may not be able to answer this question until you set about solving the problem. That's okay; it's still worth considering the question at this early stage.)
5.  How should I label the important pieces of data that are a part of the problem?

## EXPLORE EXAMPLES

-   Start with Simple Examples
-   Progress to More Complex Examples
-   Explore Examples with Empty Inputs
-   Explore Examples with Invalid Inputs

## BREAK IT DOWN


## Explicitly write out the steps you need to take. 
**This forces you to think about the code you'll write before you write it, and helps you catch any lingering conceptual issues or misunderstandings before you dive in and have to worry about details (e.g. language syntax) as well.**


## SOLVE THE PROBLEM

If you can't...

SOLVE A SIMPLER PROBLEM!

## SIMPLIFY
-   Find the core difficulty in what you're trying to do
-   Temporarily ignore that difficulty
-   Write a simplified solution
-   Then incorporate that difficulty back in
## Look back and Refactor
-   Can you check the result?
-   Can you derive the result differently?
-   Can you understand it at a glance?
-   Can you use the result or method for some other problem?
-   Can you improve the performance of your solution?
-   Can you think of other ways to refactor?
-   How have other people solved this problem?

# SOME PATTERNS...

-   Frequency Counter
-   Multiple Pointers
-   Sliding Window
-   Divide and Conquer
-   Dynamic Programming
-   Greedy Algorithms
-   Backtracking
-   **Many more!**

[Best Patterns Repo with examples and Images](https://github.com/Chanda-Abdul/Several-Coding-Patterns-for-Solving-Data-Structures-and-Algorithms-Problems-during-Interviews)

## Problem Solving Pattern Tips
**Below is a list of some useful tips and patterns that are generally helpful to solve a typical DSA problem. We know that each problem could be mapped to a pattern, and remembering these patterns will surely help you out with the correct problematic approach.**


-   If the given input is sorted, we can use binary search or the two pointer strategy to work out the solution.
-   If the problem deals with the top/min/max/closest K elements among given n elements, use a heap to simplify it.
-   When you need to try out all combinations( or permutations) of the input (given the constraints are low and suitable enough), use either the Recursive Backtracking algorithm or the Iterative BFS algorithm.
-   Most of the problems related to trees and graphs could be solved either through a DFS or BFS approach.
-   Every recursive solution can be converted to an iterative solution using stacks.
-   If for a problem there exists a brute force solution in O(n^2) time complexity and constant space, then following two can also exist:  
    1. Using a hashmap or a set for O(n) time and O(n) space.  
    2. Using sorting for O(nlogn) time and constant space.
-   When you have to optimize the solution with problems that could be divided into smaller subproblems, use a DP approach.
-   Many optimization problems also demand the knowledge of Binary Search algorithm. So if it occurs to you intuitively, you can surely crack the code within a few mins. Some typical examples include dealing with min/max/at least/at most/largest min/smallest max etc.
-   If we need to find some common substring among a set of strings, use a hashmap or a trie(prefix tree)
-   When there is a need to search among a bunch of strings, Trie will be the best data structure.
-   If problem involves a linked list and we can't use extra space, then usually its related to reversing some part of it or using a Fast and Slow pointer (Hare and Tortoise).
-   If O(n) time and O(n) space is to be reduced to O(n) time and constant space, try incorporating the two pointer method.
