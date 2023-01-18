## Description

<div><p>Sereja loves all sorts of algorithms. He has recently come up with a new algorithm, which receives a string as an input. Let's represent the input string of the algorithm as <span class="tex-span"><i>q</i> = <i>q</i><sub class="lower-index">1</sub><i>q</i><sub class="lower-index">2</sub>... <i>q</i><sub class="lower-index"><i>k</i></sub></span>. The algorithm consists of two steps:</p><ol> <li> Find any continuous subsequence (substring) of three characters of string <span class="tex-span"><i>q</i></span>, which doesn't equal to either string "<span class="tex-font-style-tt">zyx</span>", "<span class="tex-font-style-tt">xzy</span>", "<span class="tex-font-style-tt">yxz</span>". If <span class="tex-span"><i>q</i></span> doesn't contain any such subsequence, terminate the algorithm, otherwise go to step 2. </li><li> Rearrange the letters of the found subsequence randomly and go to step 1. </li></ol><p>Sereja thinks that the algorithm works correctly on string <span class="tex-span"><i>q</i></span> if there is a non-zero probability that the algorithm will be terminated. But if the algorithm anyway will work for infinitely long on a string, then we consider the algorithm to work incorrectly on this string.</p><p>Sereja wants to test his algorithm. For that, he has string <span class="tex-span"><i>s</i> = <i>s</i><sub class="lower-index">1</sub><i>s</i><sub class="lower-index">2</sub>... <i>s</i><sub class="lower-index"><i>n</i></sub></span>, consisting of <span class="tex-span"><i>n</i></span> characters. The boy conducts a series of <span class="tex-span"><i>m</i></span> tests. As the <span class="tex-span"><i>i</i></span>-th test, he sends substring <span class="tex-span"><i>s</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub></sub><i>s</i><sub class="lower-index"><i>l</i><sub class="lower-index"><i>i</i></sub> + 1</sub>... <i>s</i><sub class="lower-index"><i>r</i><sub class="lower-index"><i>i</i></sub></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> to the algorithm input. Unfortunately, the implementation of his algorithm works too long, so Sereja asked you to help. For each test <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>)</span> determine if the algorithm works correctly on this test or not.</p></div><div class="input-specification"><p>The first line contains non-empty string <span class="tex-span"><i>s</i></span>, its length (<span class="tex-span"><i>n</i></span>) doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. It is guaranteed that string <span class="tex-span"><i>s</i></span> only contains characters: '<span class="tex-font-style-tt">x</span>', '<span class="tex-font-style-tt">y</span>', '<span class="tex-font-style-tt">z</span>'.</p><p>The second line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of tests. Next <span class="tex-span"><i>m</i></span> lines contain the tests. The <span class="tex-span"><i>i</i></span>-th line contains a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p></div><div class="output-specification"><p>For each test, print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if the algorithm works correctly on the corresponding test and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p></div>

## Input

<p>The first line contains non-empty string <span class="tex-span"><i>s</i></span>, its length (<span class="tex-span"><i>n</i></span>) doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. It is guaranteed that string <span class="tex-span"><i>s</i></span> only contains characters: '<span class="tex-font-style-tt">x</span>', '<span class="tex-font-style-tt">y</span>', '<span class="tex-font-style-tt">z</span>'.</p><p>The second line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of tests. Next <span class="tex-span"><i>m</i></span> lines contain the tests. The <span class="tex-span"><i>i</i></span>-th line contains a pair of integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>.</p>

## Output

<p>For each test, print "<span class="tex-font-style-tt">YES</span>" (without the quotes) if the algorithm works correctly on the corresponding test and "<span class="tex-font-style-tt">NO</span>" (without the quotes) otherwise.</p>





```input1
zyxxxxxxyyz
5
5 5
1 3
1 11
1 4
3 6

```




```output1
YES
YES
NO
YES
NO

```



## Note

<p>In the first example, in test one and two the algorithm will always be terminated in one step. In the fourth test you can get string "<span class="tex-font-style-tt">xzyx</span>" on which the algorithm will terminate. In all other tests the algorithm doesn't work correctly. </p>
