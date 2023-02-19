## Description

<div><p><span class="tex-span"><i>n</i></span> hobbits are planning to spend the night at Frodo's house. Frodo has <span class="tex-span"><i>n</i></span> beds standing in a row and <span class="tex-span"><i>m</i></span> pillows (<span class="tex-span"><i>n</i> ≤ <i>m</i></span>). Each hobbit needs a bed and at least one pillow to sleep, however, everyone wants as many pillows as possible. Of course, it's not always possible to share pillows equally, but any hobbit gets hurt if he has at least two pillows less than some of his neighbors have. </p><p>Frodo will sleep on the <span class="tex-span"><i>k</i></span>-th bed in the row. What is the maximum number of pillows he can have so that every hobbit has at least one pillow, every pillow is given to some hobbit and no one is hurt?</p></div><div class="input-specification"><p>The only line contain three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of hobbits, the number of pillows and the number of Frodo's bed.</p></div><div class="output-specification"><p>Print single integer&nbsp;— the maximum number of pillows Frodo can have so that no one is hurt.</p></div>

## Input

<p>The only line contain three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>)&nbsp;— the number of hobbits, the number of pillows and the number of Frodo's bed.</p>

## Output

<p>Print single integer&nbsp;— the maximum number of pillows Frodo can have so that no one is hurt.</p>





```input1
4 6 2

```




```input2
3 10 3

```




```input3
3 6 1

```




```output1
2

```




```output2
4

```




```output3
3

```



## Note

<p>In the first example Frodo can have at most two pillows. In this case, he can give two pillows to the hobbit on the first bed, and one pillow to each of the hobbits on the third and the fourth beds.</p><p>In the second example Frodo can take at most four pillows, giving three pillows to each of the others.</p><p>In the third example Frodo can take three pillows, giving two pillows to the hobbit in the middle and one pillow to the hobbit on the third bed.</p>
