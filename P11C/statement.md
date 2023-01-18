## Description

<div><p>You are given a 0-1 rectangular matrix. What is the number of squares in it? A square is a solid square frame (border) with linewidth equal to 1. A square should be at least <span class="tex-span">2 × 2</span>. We are only interested in two types of squares: </p><ol> <li> squares with each side parallel to a side of the matrix; </li><li> squares with each side parallel to a diagonal of the matrix. </li></ol><pre class="verbatim"><br>For example the following matrix contains only one square of the first type: <br>0000000 <br>0111100 <br>0100100 <br>0100100 <br>0111100<br></pre><pre class="verbatim"><br>The following matrix contains only one square of the second type:<br>0000000<br>0010000<br>0101000<br>0010000<br>0000000<br></pre><p>Regardless of type, a square must contain at least one <span class="tex-font-style-tt">1</span> and can't touch (by side or corner) any foreign <span class="tex-font-style-tt">1</span>. Of course, the lengths of the sides of each square should be equal.</p><p>How many squares are in the given matrix?</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10000</span>), where <span class="tex-span"><i>t</i></span> is the number of test cases in the input. Then test cases follow. Each case starts with a line containing integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 250</span>), where <span class="tex-span"><i>n</i></span> is the number of rows and <span class="tex-span"><i>m</i></span> is the number of columns. The following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each (<span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>).</p><p>The total number of characters in all test cases doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> for any input file.</p></div><div class="output-specification"><p>You should output exactly <span class="tex-span"><i>t</i></span> lines, with the answer to the <span class="tex-span"><i>i</i></span>-th test case on the <span class="tex-span"><i>i</i></span>-th line.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10000</span>), where <span class="tex-span"><i>t</i></span> is the number of test cases in the input. Then test cases follow. Each case starts with a line containing integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i>, <i>m</i> ≤ 250</span>), where <span class="tex-span"><i>n</i></span> is the number of rows and <span class="tex-span"><i>m</i></span> is the number of columns. The following <span class="tex-span"><i>n</i></span> lines contain <span class="tex-span"><i>m</i></span> characters each (<span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>).</p><p>The total number of characters in all test cases doesn't exceed <span class="tex-span">10<sup class="upper-index">6</sup></span> for any input file.</p>

## Output

<p>You should output exactly <span class="tex-span"><i>t</i></span> lines, with the answer to the <span class="tex-span"><i>i</i></span>-th test case on the <span class="tex-span"><i>i</i></span>-th line.</p>





```input1
2
8 8
00010001
00101000
01000100
10000010
01000100
00101000
11010011
11000011
10 10
1111111000
1000001000
1011001000
1011001010
1000001101
1001001010
1010101000
1001001000
1000001000
1111111000

```




```input2
1
12 11
11111111111
10000000001
10111111101
10100000101
10101100101
10101100101
10100000101
10100000101
10111111101
10000000001
11111111111
00000000000

```




```output1
1
2

```




```output2
3

```


