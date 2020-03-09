# Writing-a-program-in-Scheme
1. Check if an input string is a palindrome, return a boolean value. Allow list input type. <br>
Required implementation: Write your own reverser function.

Example of input-output:
> (palindrome? '(1 2 3 2 1))
#t
> (palindrome? '(aa bb aa))
#t
> (palindrome? '(1 2 3 4 2 1))
#f
> 

2. Create a lambda expression that evaluates a sum of the first n-numbers of positive integers. 
Combine this lambda expression with a map so that you can pass in a list of numbers and get the sum of the first n-numbers for each number
and return a list.
3. Perform input validation (error checking).

The function "sum-positive-int" evaluates the sum of the first n-terms of the sequence of positive integers.
Map function applies the function "sum-positive-num" to each element of the list  we give it (which is the list of numbers of terms to be summed up)
The map function returns the list with all evaluated sums in it.<br>

Example of input-output:
> (map sum-positive-int '(2 3 5))   ;it returns the list with all evaluated sums: (3 6 15) 1+2=3; 1+2+3=6; 1+2+3+4+5=15;
(3 6 15)
> (map sum-positive-int '(-1 4 5))
Error! Number of terms to be evaluated should be positive(#<void> 10 15)
> (map sum-positive-int '(4))
(10)

