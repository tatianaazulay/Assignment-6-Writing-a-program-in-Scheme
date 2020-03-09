# Writing-a-program-in-Scheme
1. Check if an input string is a palindrome, return a boolean value. Allow list input type. <br>
Required implementation: Write your own reverser function.<br>

Example of input-output:<br>
> (palindrome? '(1 2 3 2 1))<br>
#t<br>
> (palindrome? '(aa bb aa))<br>
#t<br>
> (palindrome? '(1 2 3 4 2 1))<br>
#f<br>
> 

2. Create a lambda expression that evaluates a sum of the first n-numbers of positive integers. 
Combine this lambda expression with a map so that you can pass in a list of numbers and get the sum of the first n-numbers for each number and return a list.
3. Perform input validation (error checking).<br>

The function "sum-positive-int" evaluates the sum of the first n-terms of the sequence of positive integers.<br>
Map function applies the function "sum-positive-num" to each element of the list  we give it (which is the list of numbers of terms to be summed up)<br>
The map function returns the list with all evaluated sums in it.<br>

Example of input-output:<br>
> (map sum-positive-int '(2 3 5))   ;it returns the list with all evaluated sums: (3 6 15) 1+2=3; 1+2+3=6; 1+2+3+4+5=15;<br>
(3 6 15)<br>
> (map sum-positive-int '(-1 4 5))<br>
Error! Number of terms to be evaluated should be positive(#<void> 10 15)<br>
> (map sum-positive-int '(4))<br>
(10)<br>

