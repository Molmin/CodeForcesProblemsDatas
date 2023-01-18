## Description

<div><p>The Smart Beaver from ABBYY has a lot of hobbies. One of them is constructing efficient hash tables. One of the most serious problems in hash tables is resolving collisions. The Beaver is interested in this problem very much and he decided to explore it in detail.</p><p>We assume that the hash table consists of <span class="tex-span"><i>h</i></span> cells numbered from <span class="tex-span">0</span> to <span class="tex-span"><i>h</i> - 1</span>. Objects are added to and removed from it. Every object has its own unique identifier. In addition, every object has a corresponding hash value — an integer between <span class="tex-span">0</span> and <span class="tex-span"><i>h</i> - 1</span>, inclusive. When an object is added to the table, if the cell corresponding to the hash value of the object is free, then this object goes there. If the cell is already occupied by another object, there is a collision. When an object is deleted from the table, the cell which it occupied becomes empty.</p><p>The Smart Beaver has recently learned about the method of linear probing to resolve collisions. It is as follows. Let's say that the hash value for the added object equals <span class="tex-span"><i>t</i></span> and cell <span class="tex-span"><i>t</i></span> of the table is already occupied. Then we try to add this object to cell <span class="tex-span">(<i>t</i> + <i>m</i>)&nbsp;<i>mod</i>&nbsp;<i>h</i></span>. If it is also occupied, then we try cell <span class="tex-span">(<i>t</i> + 2·<i>m</i>)&nbsp;<i>mod</i>&nbsp;<i>h</i></span>, then cell <span class="tex-span">(<i>t</i> + 3·<i>m</i>)&nbsp;<i>mod</i>&nbsp;<i>h</i></span>, and so on. Note that in some cases it's possible that the new object can not be added to the table. <span class="tex-font-style-underline">It is guaranteed that the input for this problem doesn't contain such situations</span>.</p><p>The operation <span class="tex-span"><i>a</i>&nbsp;<i>mod</i>&nbsp;<i>b</i></span> means that we take the remainder of the division of number <span class="tex-span"><i>a</i></span> by number <span class="tex-span"><i>b</i></span>.</p><p>This technique immediately seemed very inoptimal to the Beaver, and he decided to assess its inefficiency. So, you are given a sequence of operations, each of which is either an addition of an object to the table or a deletion of an object from the table. When adding a new object, a sequence of calls to the table is performed. Calls to occupied cells are called dummy. In other words, if the result of the algorithm described above is the object being added to cell <span class="tex-span">(<i>t</i> + <i>i</i>·<i>m</i>)&nbsp;<i>mod</i>&nbsp;<i>h</i></span> <span class="tex-span">(<i>i</i> ≥ 0)</span>, then exactly <span class="tex-span"><i>i</i></span> dummy calls have been performed.</p><p>Your task is to calculate the total number of dummy calls to the table for the given sequence of additions and deletions. When an object is deleted from the table, assume that no dummy calls are performed. The table is empty before performing the operations, that is, initially it doesn't contain any objects.</p></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i> &lt; <i>h</i></span>), separated by spaces, where <span class="tex-span"><i>h</i></span> is the size of the hash table, <span class="tex-span"><i>m</i></span> is the number that is used to resolve collisions, <span class="tex-span"><i>n</i></span> is the number of operations.</p><p>The following <span class="tex-span"><i>n</i></span> lines contains the descriptions of the operations. Their execution order corresponds to the order in which they appear in the input file. Each operation is described by a single line. The operations are described as follows:</p><ul> <li> "<span class="tex-font-style-tt">+ id hash</span>"<p>This is the format of the operation that adds an object to the table. The first character is "<span class="tex-font-style-tt">+</span>" (ASCII 43), followed by a single space, then the object identifier <span class="tex-span"><i>id</i></span> <span class="tex-span">(0 ≤ <i>id</i> ≤ 10<sup class="upper-index">9</sup>)</span>, then another space, and the hash value of the given object <span class="tex-span"><i>hash</i></span> <span class="tex-span">(0 ≤ <i>hash</i> &lt; <i>h</i>)</span>. The object identifier and the hash value of this object are integers.</p></li><li> "<span class="tex-font-style-tt">- id</span>"<p>This is the format of the operation that deletes an object from the table. The first character is "<span class="tex-font-style-tt">-</span>" (ASCII 45), followed by a single space, then the object identifier <span class="tex-span"><i>id</i></span> <span class="tex-span">(0 ≤ <i>id</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The object identifier is an integer.</p></li></ul><p>It is guaranteed that for all addition operations the value of <span class="tex-span"><i>id</i></span> is unique. It is also guaranteed that the initial data is correct, that is, it's always possible to add an object to the hash table and there won't be any deletions of nonexisting objects.</p><p>The input limitations for getting 20 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>h</i> ≤ 5000</span> </li><li> <span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span> </li></ul><p>The input limitations for getting 50 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>h</i> ≤ 5·10<sup class="upper-index">4</sup></span> </li><li> <span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span> </li></ul><p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>h</i> ≤ 2·10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span> </li></ul></div><div class="output-specification"><p>Print a single number — the total number of dummy calls to the hash table.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams and the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>h</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>m</i> &lt; <i>h</i></span>), separated by spaces, where <span class="tex-span"><i>h</i></span> is the size of the hash table, <span class="tex-span"><i>m</i></span> is the number that is used to resolve collisions, <span class="tex-span"><i>n</i></span> is the number of operations.</p><p>The following <span class="tex-span"><i>n</i></span> lines contains the descriptions of the operations. Their execution order corresponds to the order in which they appear in the input file. Each operation is described by a single line. The operations are described as follows:</p><ul> <li> "<span class="tex-font-style-tt">+ id hash</span>"<p>This is the format of the operation that adds an object to the table. The first character is "<span class="tex-font-style-tt">+</span>" (ASCII 43), followed by a single space, then the object identifier <span class="tex-span"><i>id</i></span> <span class="tex-span">(0 ≤ <i>id</i> ≤ 10<sup class="upper-index">9</sup>)</span>, then another space, and the hash value of the given object <span class="tex-span"><i>hash</i></span> <span class="tex-span">(0 ≤ <i>hash</i> &lt; <i>h</i>)</span>. The object identifier and the hash value of this object are integers.</p></li><li> "<span class="tex-font-style-tt">- id</span>"<p>This is the format of the operation that deletes an object from the table. The first character is "<span class="tex-font-style-tt">-</span>" (ASCII 45), followed by a single space, then the object identifier <span class="tex-span"><i>id</i></span> <span class="tex-span">(0 ≤ <i>id</i> ≤ 10<sup class="upper-index">9</sup>)</span>. The object identifier is an integer.</p></li></ul><p>It is guaranteed that for all addition operations the value of <span class="tex-span"><i>id</i></span> is unique. It is also guaranteed that the initial data is correct, that is, it's always possible to add an object to the hash table and there won't be any deletions of nonexisting objects.</p><p>The input limitations for getting 20 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>h</i> ≤ 5000</span> </li><li> <span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span> </li></ul><p>The input limitations for getting 50 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>h</i> ≤ 5·10<sup class="upper-index">4</sup></span> </li><li> <span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">4</sup></span> </li></ul><p>The input limitations for getting 100 points are: </p><ul> <li> <span class="tex-span">1 ≤ <i>h</i> ≤ 2·10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span> </li></ul>

## Output

<p>Print a single number — the total number of dummy calls to the hash table.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams and the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
10 2 7
+ 11 0
+ 22 2
+ 33 6
+ 44 0
+ 55 0
- 22
+ 66 0

```




```input2
5 1 6
+ 123 0
+ 234 1
+ 345 2
- 234
+ 456 0
+ 567 0

```




```output1
7

```




```output2
4

```


