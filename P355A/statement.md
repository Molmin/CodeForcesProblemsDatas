## Description

<div><p>Vasya has recently found out what a digital root of a number is and he decided to share his knowledge with you.</p><p>Let's assume that <span class="tex-span"><i>S</i>(<i>n</i>)</span> is the sum of digits of number <span class="tex-span"><i>n</i></span>, for example, <span class="tex-span"><i>S</i>(4098) = 4 + 0 + 9 + 8 = 21</span>. Then the digital root of number <span class="tex-span"><i>n</i></span> equals to: </p><ol> <li> <span class="tex-span"><i>dr</i>(<i>n</i>) = <i>S</i>(<i>n</i>)</span>, if <span class="tex-span"><i>S</i>(<i>n</i>) &lt; 10</span>; </li><li> <span class="tex-span"><i>dr</i>(<i>n</i>) = <i>dr</i>( <i>S</i>(<i>n</i>) )</span>, if <span class="tex-span"><i>S</i>(<i>n</i>) ≥ 10</span>. </li></ol><p>For example, <span class="tex-span"><i>dr</i>(4098)  =  <i>dr</i>(21)  =  3</span>.</p><p>Vasya is afraid of large numbers, so the numbers he works with are at most <span class="tex-span">10<sup class="upper-index">1000</sup></span>. For all such numbers, he has proved that <span class="tex-span"><i>dr</i>(<i>n</i>)  =  <i>S</i>( <i>S</i>( <i>S</i>( <i>S</i>(<i>n</i>) ) ) )</span> <span class="tex-span">(<i>n</i> ≤ 10<sup class="upper-index">1000</sup>)</span>.</p><p>Now Vasya wants to quickly find numbers with the given digital root. The problem is, he hasn't learned how to do that and he asked you to help him. You task is, given numbers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>d</i></span>, find the number consisting of exactly <span class="tex-span"><i>k</i></span> digits (the leading zeroes are not allowed), with digital root equal to <span class="tex-span"><i>d</i></span>, or else state that such number does not exist.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 1000; 0 ≤ <i>d</i> ≤ 9)</span>.</p></div><div class="output-specification"><p>In a single line print either any number that meets the requirements (without the leading zeroes) or "<span class="tex-font-style-tt">No solution</span>" (without the quotes), if the corresponding number does not exist.</p><p>The chosen number must consist of exactly <span class="tex-span"><i>k</i></span> digits. We assume that number 0 doesn't contain any leading zeroes.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>k</i> ≤ 1000; 0 ≤ <i>d</i> ≤ 9)</span>.</p>

## Output

<p>In a single line print either any number that meets the requirements (without the leading zeroes) or "<span class="tex-font-style-tt">No solution</span>" (without the quotes), if the corresponding number does not exist.</p><p>The chosen number must consist of exactly <span class="tex-span"><i>k</i></span> digits. We assume that number 0 doesn't contain any leading zeroes.</p>





```input1
4 4

```




```input2
5 1

```




```input3
1 0

```




```output1
5881

```




```output2
36172

```




```output3
0

```



## Note

<p>For the first test sample <span class="tex-span"><i>dr</i>(5881)  =  <i>dr</i>(22)  =  4</span>.</p><p>For the second test sample <span class="tex-span"><i>dr</i>(36172)  =  <i>dr</i>(19)  =  <i>dr</i>(10)  =  1</span>.</p>
