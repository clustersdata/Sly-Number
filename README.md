# Sly-Number

Sly Number

Description

Let's consider so called "sly number" which is given as an array A of N integers from set {0,1,2}. For example A[0]=1, A[1]=1, A[2]=0 and A[3]=2. A sly number is called ONE, if A[0]=1 and A[I]=0 for I=1,2,?,N-1. 
Consider following operation with two sly numbers A and B called 'Star Multiplication': 

                                  k                             N-1

                    C[k]     =   ∑  A[i] * B[k-i]      +       ∑  A[i] * B[N+k-i].

                                 i=0                           i=k+1


here C ? the result of the operation, even also presented in an array - not necessarily sly number. This operation we will denote by <*> symbol. 

Moreover, there is also module operation over the results of 'Star Multiplication': 

                                         (C mod Q) [i]     =     C[i] mod Q,


where Q is a positive integer. 

We are given a sly number A and a module Q. We need to find such 'inverse sly number' B: 

(A * B) mod Q = ONE.

Input

The input contains K data sets in text format. The first line of this file contains the number K of test cases. Each test consists of two lines. First line contains two integers separated by spaces: Q (2 <= Q <= 100) and N (5 <= N <= 50). Second line contains N integers from set {0,1,2} separated by spaces, which present sly number A.

Output

The output should be printed on the standard output. It should contain K lines - one line for each test case. If a solution exists, the line should contain the string "A solution can be found". In case there is no solution, the line should consist of string 'No solution'.

Sample Input

2
2 5
1 0 1 0 1
65 8
1 2 2 2 1 1 2 2

Sample Output

A solution can be found
No solution

Hint

In the first sample one possible inverse sly number could be <0 0 1 1 1>.
