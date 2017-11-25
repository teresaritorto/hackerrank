# Append and Delete Problem

You have a string, , of lowercase English alphabetic letters. You can perform two types of operations on :

Append a lowercase English alphabetic letter to the end of the string.
Delete the last character in the string. Performing this operation on an empty string results in an empty string.
Given an integer, , and two strings,  and , determine whether or not you can convert  to  by performing exactly  of the above operations on . If it's possible, print Yes; otherwise, print No.


#### Input Format

The first line contains a string, , denoting the initial string. 
The second line contains a string, , denoting the desired final string. The third line contains an integer, , denoting the desired number of operations.

#### Constraints
* s & t consist of lowercase English alphabetic letters

#### Output Format
Print Yes if you can obtain string  by performing exactly  operations on ; otherwise, print No.

 and  consist of lowercase English alphabetic letters.
Output Format

#### Sample Input 0

hackerhappy
hackerrank
9

#### Sample Output 0
Yes

#### Explanation 0
We perform  delete operations to reduce string  to hacker. Next, we perform  append operations (i.e., r, a, n, and k), to get hackerrank. Because we were able to convert  to by performing exactly  operations, we print Yes.
