## Description

<div><p>Little Petya likes arrays of integers a lot. Recently his mother has presented him one such array consisting of <span class="tex-span"><i>n</i></span> elements. Petya is now wondering whether he can swap any two distinct integers in the array so that the array got unsorted. Please note that Petya can not swap equal integers even if they are in distinct positions in the array. Also note that Petya <span class="tex-font-style-bf">must</span> swap some two integers even if the original array meets all requirements.</p><p>Array <span class="tex-span"><i>a</i></span> (the array elements are indexed from 1) consisting of <span class="tex-span"><i>n</i></span> elements is called sorted if it meets at least one of the following two conditions:</p><ol> <li> <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> ≤ <i>a</i><sub class="lower-index">2</sub> ≤ ... ≤ <i>a</i><sub class="lower-index"><i>n</i></sub></span>; </li><li> <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> ≥ <i>a</i><sub class="lower-index">2</sub> ≥ ... ≥ <i>a</i><sub class="lower-index"><i>n</i></sub></span>. </li></ol><p>Help Petya find the two required positions to swap or else say that they do not exist.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> non-negative space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> — the elements of the array that Petya's mother presented him. All integers in the input do not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p></div><div class="output-specification"><p>If there is a pair of positions that make the array unsorted if swapped, then print the numbers of these positions separated by a space. If there are several pairs of positions, print any of them. If such pair does not exist, print -1. The positions in the array are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> non-negative space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> — the elements of the array that Petya's mother presented him. All integers in the input do not exceed <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p>

## Output

<p>If there is a pair of positions that make the array unsorted if swapped, then print the numbers of these positions separated by a space. If there are several pairs of positions, print any of them. If such pair does not exist, print -1. The positions in the array are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p>





```input1
1
1

```




```input2
2
1 2

```




```input3
4
1 2 3 4

```




```input4
3
1 1 1

```




```output1
-1

```




```output2
-1

```




```output3
1 2

```




```output4
-1

```



## Note

<p>In the first two samples the required pairs obviously don't exist.</p><p>In the third sample you can swap the first two elements. After that the array will look like this: <span class="tex-font-style-tt">2 1 3 4</span>. This array is unsorted.</p>
