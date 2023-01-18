## Description

<div><p>Little Petya likes numbers a lot. Recently his mother has presented him a collection of <span class="tex-span"><i>n</i></span> non-negative integers. There's only one thing Petya likes more than numbers: playing with little Masha. He immediately decided to give a part of his new collection to her. To make the game even more interesting, Petya decided to give Masha such collection of numbers for which the following conditions fulfill:</p><ul> <li> Let's introduce <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span> to denote the <span class="tex-span"><i>xor</i></span> of all numbers Petya has got left; and let's introduce <span class="tex-span"><i>x</i><sub class="lower-index">2</sub></span> to denote the <span class="tex-span"><i>xor</i></span> of all numbers he gave to Masha. Value <span class="tex-span">(<i>x</i><sub class="lower-index">1</sub> + <i>x</i><sub class="lower-index">2</sub>)</span> must be as large as possible. </li><li> If there are multiple ways to divide the collection so that the previous condition fulfilled, then Petya minimizes the value <span class="tex-span"><i>x</i><sub class="lower-index">1</sub></span>. </li></ul><p>The <span class="tex-span"><i>xor</i></span> operation is a bitwise excluding "<span class="tex-font-style-tt">OR</span>", that is denoted as "<span class="tex-font-style-tt">xor</span>" in the Pascal language and "<span class="tex-font-style-tt">^</span>" in C/C++/Java.</p><p>Help Petya divide the collection as described above. If there are multiple suitable ways to divide it, find any of them. Please note that after Petya gives a part of his numbers to Masha, he may have no numbers left. The reverse situation is also possible, when Petya gives nothing to Masha. In both cases we must assume that the <span class="tex-span"><i>xor</i></span> of an empty set of numbers equals 0.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), showing how many numbers Petya's mother gave him. The second line contains the actual space-separated numbers. They are all integer, non-negative and do not exceed <span class="tex-span">10<sup class="upper-index">18</sup></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> space-separated integers, the <span class="tex-span"><i>i</i></span>-th of them should equal either 1, if Petya keeps the number that follows <span class="tex-span"><i>i</i></span>-th in his collection, or it should equal 2, if Petya gives the corresponding number to Masha. The numbers are indexed in the order in which they are given in the input.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), showing how many numbers Petya's mother gave him. The second line contains the actual space-separated numbers. They are all integer, non-negative and do not exceed <span class="tex-span">10<sup class="upper-index">18</sup></span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> space-separated integers, the <span class="tex-span"><i>i</i></span>-th of them should equal either 1, if Petya keeps the number that follows <span class="tex-span"><i>i</i></span>-th in his collection, or it should equal 2, if Petya gives the corresponding number to Masha. The numbers are indexed in the order in which they are given in the input.</p>





```input1
6
1 2 3 4 5 6

```




```input2
3
1000000000000 1000000000000 1000000000000

```




```input3
8
1 1 2 2 3 3 4 4

```




```output1
2 2 2 2 2 2

```




```output2
2 2 2

```




```output3
1 2 1 2 2 2 1 2

```


