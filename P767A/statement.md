## Description

<div><p>According to an old legeng, a long time ago Ankh-Morpork residents did something wrong to miss Fortune, and she cursed them. She said that at some time <span class="tex-span"><i>n</i></span> snacks of distinct sizes will fall on the city, and the residents should build a Snacktower of them by placing snacks one on another. Of course, big snacks should be at the bottom of the tower, while small snacks should be at the top.</p><p>Years passed, and once different snacks started to fall onto the city, and the residents began to build the Snacktower.</p><center> <img class="tex-graphics" height="318px" src="file://45kFdBek.png" style="max-width: 100.0%;max-height: 100.0%;" width="265px"> </center><p>However, they faced some troubles. Each day exactly one snack fell onto the city, but their order was strange. So, at some days the residents weren't able to put the new stack on the top of the Snacktower: they had to wait until all the bigger snacks fell. Of course, in order to not to anger miss Fortune again, the residents placed each snack on the top of the tower immediately as they could do it.</p><p>Write a program that models the behavior of Ankh-Morpork residents.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the total number of snacks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them equals the size of the snack which fell on the <span class="tex-span"><i>i</i></span>-th day. Sizes are distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. On the <span class="tex-span"><i>i</i></span>-th of them print the sizes of the snacks which the residents placed on the top of the Snacktower on the <span class="tex-span"><i>i</i></span>-th day in the order they will do that. If no snack is placed on some day, leave the corresponding line empty.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the total number of snacks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them equals the size of the snack which fell on the <span class="tex-span"><i>i</i></span>-th day. Sizes are distinct integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. </p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. On the <span class="tex-span"><i>i</i></span>-th of them print the sizes of the snacks which the residents placed on the top of the Snacktower on the <span class="tex-span"><i>i</i></span>-th day in the order they will do that. If no snack is placed on some day, leave the corresponding line empty.</p>





```input1
3
3 1 2

```




```input2
5
4 5 1 2 3

```




```output1
3
&nbsp;
2 1
```




```output2
&nbsp;
5 4
&nbsp;
&nbsp;
3 2 1

```



## Note

<p>In the example a snack of size <span class="tex-span">3</span> fell on the first day, and the residents immediately placed it. On the second day a snack of size <span class="tex-span">1</span> fell, and the residents weren't able to place it because they were missing the snack of size <span class="tex-span">2</span>. On the third day a snack of size <span class="tex-span">2</span> fell, and the residents immediately placed it. Right after that they placed the snack of size <span class="tex-span">1</span> which had fallen before.</p>
