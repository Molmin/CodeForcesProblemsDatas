## Description

<div><p>In one well-known algorithm of finding the <span class="tex-span"><i>k</i></span>-th order statistics we should divide all elements into groups of five consecutive elements and find the median of each five. A median is called the middle element of a sorted array (it's the third largest element for a group of five). To increase the algorithm's performance speed on a modern video card, you should be able to find a sum of medians in each five of the array.</p><p>A <span class="tex-font-style-it">sum of medians</span> of a sorted <span class="tex-span"><i>k</i></span>-element set <span class="tex-span"><i>S</i> = {<i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub>}</span>, where <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> &lt; <i>a</i><sub class="lower-index">2</sub> &lt; <i>a</i><sub class="lower-index">3</sub> &lt; ... &lt; <i>a</i><sub class="lower-index"><i>k</i></sub></span>, will be understood by as </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://A21M7wya.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>The <img align="middle" class="tex-formula" src="file://uPdvvQUV.png" style="max-width: 100.0%;max-height: 100.0%;"> operator stands for taking the remainder, that is <img align="middle" class="tex-formula" src="file://s102HAQW.png" style="max-width: 100.0%;max-height: 100.0%;"> stands for the remainder of dividing <span class="tex-span"><i>x</i></span> by <span class="tex-span"><i>y</i></span>.</p><p>To organize exercise testing quickly calculating <span class="tex-font-style-it">the sum of medians</span> for a changing set was needed.</p></div><div class="input-specification"><p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of operations performed.</p><p>Then each of <span class="tex-span"><i>n</i></span> lines contains the description of one of the three operations: </p><ul> <li> <span class="tex-font-style-tt">add <span class="tex-span"><i>x</i></span></span>&nbsp;— add the element <span class="tex-span"><i>x</i></span> to the set; </li><li> <span class="tex-font-style-tt">del <span class="tex-span"><i>x</i></span></span>&nbsp;— delete the element <span class="tex-span"><i>x</i></span> from the set; </li><li> <span class="tex-font-style-tt">sum</span>&nbsp;— find the <span class="tex-font-style-it">sum of medians</span> of the set. </li></ul><p>For any <span class="tex-font-style-tt">add <span class="tex-span"><i>x</i></span></span> operation it is true that the element <span class="tex-span"><i>x</i></span> is not included in the set directly before the operation.</p><p>For any <span class="tex-font-style-tt">del <span class="tex-span"><i>x</i></span></span> operation it is true that the element <span class="tex-span"><i>x</i></span> is included in the set directly before the operation.</p><p>All the numbers in the input are positive integers, not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div><div class="output-specification"><p>For each operation <span class="tex-font-style-tt">sum</span> print on the single line <span class="tex-font-style-it">the sum of medians</span> of the current set. If the set is empty, print 0.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams (also you may use the <span class="tex-font-style-tt">%I64d</span> specificator).</p></div>

## Input

<p>The first line contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of operations performed.</p><p>Then each of <span class="tex-span"><i>n</i></span> lines contains the description of one of the three operations: </p><ul> <li> <span class="tex-font-style-tt">add <span class="tex-span"><i>x</i></span></span>&nbsp;— add the element <span class="tex-span"><i>x</i></span> to the set; </li><li> <span class="tex-font-style-tt">del <span class="tex-span"><i>x</i></span></span>&nbsp;— delete the element <span class="tex-span"><i>x</i></span> from the set; </li><li> <span class="tex-font-style-tt">sum</span>&nbsp;— find the <span class="tex-font-style-it">sum of medians</span> of the set. </li></ul><p>For any <span class="tex-font-style-tt">add <span class="tex-span"><i>x</i></span></span> operation it is true that the element <span class="tex-span"><i>x</i></span> is not included in the set directly before the operation.</p><p>For any <span class="tex-font-style-tt">del <span class="tex-span"><i>x</i></span></span> operation it is true that the element <span class="tex-span"><i>x</i></span> is included in the set directly before the operation.</p><p>All the numbers in the input are positive integers, not exceeding <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p>

## Output

<p>For each operation <span class="tex-font-style-tt">sum</span> print on the single line <span class="tex-font-style-it">the sum of medians</span> of the current set. If the set is empty, print 0.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams (also you may use the <span class="tex-font-style-tt">%I64d</span> specificator).</p>





```input1
6
add 4
add 5
add 1
add 2
add 3
sum

```




```input2
14
add 1
add 7
add 2
add 5
sum
add 6
add 8
add 9
add 3
add 4
add 10
sum
del 1
sum

```




```output1
3

```




```output2
5
11
13

```


