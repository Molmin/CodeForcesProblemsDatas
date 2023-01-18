## Description

<div><p><span class="tex-font-style-it">You will receive 5 points for solving this problem.</span></p><p>Manao has invented a new operation on strings that is called folding. Each fold happens between a pair of consecutive letters and places the second part of the string above first part, running in the opposite direction and aligned to the position of the fold. Using this operation, Manao converts the string into a structure that has one more level than there were fold operations performed. See the following examples for clarity.</p><p>We will denote the positions of folds with '<span class="tex-font-style-tt">|</span>' characters. For example, the word "<span class="tex-font-style-tt">ABRACADABRA</span>" written as "<span class="tex-font-style-tt">AB|RACA|DAB|RA</span>" indicates that it has been folded three times: first, between the leftmost pair of '<span class="tex-font-style-tt">B</span>' and '<span class="tex-font-style-tt">R</span>' letters; second, between '<span class="tex-font-style-tt">A</span>' and '<span class="tex-font-style-tt">D</span>'; and third, between the rightmost pair of '<span class="tex-font-style-tt">B</span>' and '<span class="tex-font-style-tt">R</span>' letters. Here are several examples of folded strings:</p><pre class="verbatim"><br>"ABCDEF|GHIJK" |  "A|BCDEFGHIJK" |  "AB|RACA|DAB|RA" |  "X|XXXXX|X|X|XXXXXX"<br>               |                 |                   |       XXXXXX<br>    KJIHG      |   KJIHGFEDCB    |      AR           |       X<br>   ABCDEF      |            A    |     DAB           |       X<br>               |                 |     ACAR          |       XXXXX<br>               |                 |       AB          |           X<br></pre><p>One last example for "<span class="tex-font-style-tt">ABCD|EFGH|IJ|K</span>": </p><pre class="verbatim"><br> K<br>IJ<br>HGFE<br>ABCD<br></pre><p>Manao noticed that each folded string can be viewed as several piles of letters. For instance, in the previous example, there are four piles, which can be read as "<span class="tex-font-style-tt">AHI</span>", "<span class="tex-font-style-tt">BGJK</span>", "<span class="tex-font-style-tt">CF</span>", and "<span class="tex-font-style-tt">DE</span>" from bottom to top. Manao wonders what is the highest pile of identical letters he can build using fold operations on a given word. Note that the pile should not contain gaps and should start at the bottom level. For example, in the rightmost of the four examples above, none of the piles would be considered valid since each of them has gaps, starts above the bottom level, or both.</p></div><div class="input-specification"><p>The input will consist of one line containing a single string of <span class="tex-span"><i>n</i></span> characters with <span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span> and no spaces. All characters of the string will be uppercase letters.</p><p><span class="tex-font-style-it">This problem doesn't have subproblems. You will get 5 points for the correct submission.</span></p></div><div class="output-specification"><p>Print a single integer — the size of the largest pile composed of identical characters that can be seen in a valid result of folding operations on the given string.</p></div>

## Input

<p>The input will consist of one line containing a single string of <span class="tex-span"><i>n</i></span> characters with <span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span> and no spaces. All characters of the string will be uppercase letters.</p><p><span class="tex-font-style-it">This problem doesn't have subproblems. You will get 5 points for the correct submission.</span></p>

## Output

<p>Print a single integer — the size of the largest pile composed of identical characters that can be seen in a valid result of folding operations on the given string.</p>





```input1
ABRACADABRA

```




```input2
ABBBCBDB

```




```input3
AB

```




```output1
3

```




```output2
3

```




```output3
1

```



## Note

<p>Consider the first example. Manao can create a pile of three '<span class="tex-font-style-tt">A</span>'s using the folding "<span class="tex-font-style-tt">AB|RACAD|ABRA</span>", which results in the following structure: </p><pre class="verbatim"><br>ABRA<br>DACAR<br>   AB<br></pre><p>In the second example, Manao can create a pile of three '<span class="tex-font-style-tt">B</span>'s using the following folding: "<span class="tex-font-style-tt">AB|BB|CBDB</span>". </p><pre class="verbatim"><br>CBDB<br>BB<br>AB<br></pre><p>Another way for Manao to create a pile of three '<span class="tex-font-style-tt">B</span>'s with "<span class="tex-font-style-tt">ABBBCBDB</span>" is the following folding: "<span class="tex-font-style-tt">AB|B|BCBDB</span>". </p><pre class="verbatim"><br> BCBDB<br> B<br>AB<br></pre><p>In the third example, there are no folds performed and the string is just written in one line.</p>
