## Description

<div><p>Once upon a time in the Kingdom of Far Far Away lived Sam the Farmer. Sam had a cow named Dawn and he was deeply attached to her. Sam would spend the whole summer stocking hay to feed Dawn in winter. Sam scythed hay and put it into haystack. As Sam was a bright farmer, he tried to make the process of storing hay simpler and more convenient to use. He collected the hay into cubical hay blocks of the same size. Then he stored the blocks in his barn. After a summer spent in hard toil Sam stored <span class="tex-span"><i>A</i>·<i>B</i>·<i>C</i></span> hay blocks and stored them in a barn as a rectangular parallelepiped <span class="tex-span"><i>A</i></span> layers high. Each layer had <span class="tex-span"><i>B</i></span> rows and each row had <span class="tex-span"><i>C</i></span> blocks.</p><p>At the end of the autumn Sam came into the barn to admire one more time the hay he'd been stacking during this hard summer. Unfortunately, Sam was horrified to see that the hay blocks had been carelessly scattered around the barn. The place was a complete mess. As it turned out, thieves had sneaked into the barn. They completely dissembled and took away a layer of blocks from the parallelepiped's front, back, top and sides. As a result, the barn only had a parallelepiped containing <span class="tex-span">(<i>A</i> - 1) × (<i>B</i> - 2) × (<i>C</i> - 2)</span> hay blocks. To hide the evidence of the crime, the thieves had dissembled the parallelepiped into single <span class="tex-span">1 × 1 × 1</span> blocks and scattered them around the barn. After the theft Sam counted <span class="tex-span"><i>n</i></span> hay blocks in the barn but he forgot numbers <span class="tex-span"><i>A</i></span>, <span class="tex-span"><i>B</i></span> и <span class="tex-span"><i>C</i></span>.</p><p>Given number <span class="tex-span"><i>n</i></span>, find the minimally possible and maximally possible number of stolen hay blocks.</p></div><div class="input-specification"><p>The only line contains integer <span class="tex-span"><i>n</i></span> from the problem's statement (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print space-separated minimum and maximum number of hay blocks that could have been stolen by the thieves.</p><p>Note that the answer to the problem can be large enough, so you must use the 64-bit integer type for calculations. Please, do not use the %lld specificator to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the %I64d specificator.</p></div>

## Input

<p>The only line contains integer <span class="tex-span"><i>n</i></span> from the problem's statement (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>

## Output

<p>Print space-separated minimum and maximum number of hay blocks that could have been stolen by the thieves.</p><p>Note that the answer to the problem can be large enough, so you must use the 64-bit integer type for calculations. Please, do not use the %lld specificator to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the %I64d specificator.</p>





```input1
4

```




```input2
7

```




```input3
12

```




```output1
28 41

```




```output2
47 65

```




```output3
48 105

```



## Note

<p>Let's consider the first sample test. If initially Sam has a parallelepiped consisting of <span class="tex-span">32 = 2 × 4 × 4</span> hay blocks in his barn, then after the theft the barn has <span class="tex-span">4 = (2 - 1) × (4 - 2) × (4 - 2)</span> hay blocks left. Thus, the thieves could have stolen <span class="tex-span">32 - 4 = 28</span> hay blocks. If Sam initially had a parallelepiped consisting of <span class="tex-span">45 = 5 × 3 × 3</span> hay blocks in his barn, then after the theft the barn has <span class="tex-span">4 = (5 - 1) × (3 - 2) × (3 - 2)</span> hay blocks left. Thus, the thieves could have stolen <span class="tex-span">45 - 4 = 41</span> hay blocks. No other variants of the blocks' initial arrangement (that leave Sam with exactly 4 blocks after the theft) can permit the thieves to steal less than 28 or more than 41 blocks.</p>
