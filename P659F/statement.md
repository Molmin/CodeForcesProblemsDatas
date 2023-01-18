## Description

<div><p>The farmer Polycarp has a warehouse with hay, which can be represented as an <span class="tex-span"><i>n</i> × <i>m</i></span> rectangular table, where <span class="tex-span"><i>n</i></span> is the number of rows, and <span class="tex-span"><i>m</i></span> is the number of columns in the table. Each cell of the table contains a haystack. The height in meters of the hay located in the <span class="tex-span"><i>i</i></span>-th row and the <span class="tex-span"><i>j</i></span>-th column is equal to an integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> and coincides with the number of cubic meters of hay in the haystack, because all cells have the size of the base <span class="tex-span">1 × 1</span>. Polycarp has decided to tidy up in the warehouse by removing an arbitrary integer amount of cubic meters of hay from the top of each stack. You can take different amounts of hay from different haystacks. Besides, it is allowed not to touch a stack at all, or, on the contrary, to remove it completely. If a stack is completely removed, the corresponding cell becomes empty and no longer contains the stack.</p><p>Polycarp wants the following requirements to hold after the reorganization:</p><ul> <li> the total amount of hay remaining in the warehouse must be <span class="tex-font-style-bf">equal</span> to <span class="tex-span"><i>k</i></span>, </li><li> the heights of all stacks (i.e., cells containing a non-zero amount of hay) should be the same, </li><li> the height of at least one stack must remain the same as it was, </li><li> for the stability of the remaining structure all the stacks should form one connected region. </li></ul><p>The two stacks are considered adjacent if they share a side in the table. The area is called connected if from any of the stack in the area you can get to any other stack in this area, moving only to adjacent stacks. In this case two adjacent stacks necessarily belong to the same area.</p><p>Help Polycarp complete this challenging task or inform that it is impossible.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of rows and columns of the rectangular table where heaps of hay are lain and the required total number cubic meters of hay after the reorganization. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each containing <span class="tex-span"><i>m</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is equal to the number of cubic meters of hay making the hay stack on the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column of the table.</p></div><div class="output-specification"><p>In the first line print "<span class="tex-font-style-tt">YES</span>" (without quotes), if Polycarpus can perform the reorganisation and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise. If the answer is "<span class="tex-font-style-tt">YES</span>" (without quotes), then in next <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>m</i></span> numbers&nbsp;— the heights of the remaining hay stacks. All the remaining non-zero values should be equal, represent a connected area and at least one of these values shouldn't be altered.</p><p>If there are multiple answers, print any of them.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>)&nbsp;— the number of rows and columns of the rectangular table where heaps of hay are lain and the required total number cubic meters of hay after the reorganization. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each containing <span class="tex-span"><i>m</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> is equal to the number of cubic meters of hay making the hay stack on the <span class="tex-span"><i>i</i></span>-th row and <span class="tex-span"><i>j</i></span>-th column of the table.</p>

## Output

<p>In the first line print "<span class="tex-font-style-tt">YES</span>" (without quotes), if Polycarpus can perform the reorganisation and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise. If the answer is "<span class="tex-font-style-tt">YES</span>" (without quotes), then in next <span class="tex-span"><i>n</i></span> lines print <span class="tex-span"><i>m</i></span> numbers&nbsp;— the heights of the remaining hay stacks. All the remaining non-zero values should be equal, represent a connected area and at least one of these values shouldn't be altered.</p><p>If there are multiple answers, print any of them.</p>





```input1
2 3 35
10 4 9
9 9 7

```




```input2
4 4 50
5 9 1 1
5 1 1 5
5 1 5 5
5 5 7 1

```




```input3
2 4 12
1 1 3 1
1 6 2 4

```




```output1
YES
7 0 7 
7 7 7 

```




```output2
YES
5 5 0 0 
5 0 0 5 
5 0 5 5 
5 5 5 0 

```




```output3
NO

```



## Note

<p>In the first sample non-zero values make up a connected area, their values do not exceed the initial heights of hay stacks. All the non-zero values equal <span class="tex-span">7</span>, and their number is <span class="tex-span">5</span>, so the total volume of the remaining hay equals the required value <span class="tex-span"><i>k</i> = 7·5 = 35</span>. At that the stack that is on the second line and third row remained unaltered.</p>
