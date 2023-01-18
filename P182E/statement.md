## Description

<div><p>Vasya has recently bought some land and decided to surround it with a wooden fence.</p><p>He went to a company called "Wooden board" that produces wooden boards for fences. Vasya read in the catalog of products that the company has at its disposal <span class="tex-span"><i>n</i></span> different types of wood. The company uses the <span class="tex-span"><i>i</i></span>-th type of wood to produce a board of this type that is a rectangular <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> by <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> block.</p><p>Vasya decided to order boards in this company and build a fence from them. It turned out that the storehouse of the company is so large that Vasya can order arbitrary number of boards of every type. Note that Vasya is allowed to <span class="tex-font-style-bf">turn</span> the boards as he builds the fence. <span class="tex-font-style-bf">However, Vasya cannot turn square boards.</span></p><p>Vasya is required to construct a fence of length <span class="tex-span"><i>l</i></span>, however, an arbitrary fence won't do. Vasya wants his fence to look beautiful. We'll say that a fence is <span class="tex-font-style-bf">beautiful</span> if and only if the following two conditions are fulfilled:</p><ul> <li> <span class="tex-font-style-bf">there are no</span> two successive boards of the same type </li><li> the first board of the fence has an arbitrary length, and the <span class="tex-font-style-bf">length</span> of each subsequent board equals the <span class="tex-font-style-bf">width</span> of the previous one </li></ul><p>In other words, the fence is considered beautiful, if the type of the <span class="tex-span"><i>i</i></span>-th board in the fence is different from the <span class="tex-span"><i>i</i> - 1</span>-th board's type; besides, the <span class="tex-span"><i>i</i></span>-th board's length is equal to the <span class="tex-span"><i>i</i> - 1</span>-th board's width (for all <span class="tex-span"><i>i</i></span>, starting from 2).</p><p>Now Vasya wonders, how many variants of arranging a fence for his land exist. Your task is to count the number of different beautiful fences of length <span class="tex-span"><i>l</i></span>.</p><p><span class="tex-font-style-bf">Two fences will be considered the same if the corresponding sequences of fence boards types and rotations are the same, otherwise the fences are different.</span> Since the sought number can be large enough, you need to calculate the answer modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 1 ≤ <i>l</i> ≤ 3000</span>) — the number of different board types and the fence length, correspondingly. Next <span class="tex-span"><i>n</i></span> lines contain descriptions of board types: the <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the sizes of the board of the <span class="tex-span"><i>i</i></span>-th type. All numbers on the lines are separated by spaces.</p></div><div class="output-specification"><p>Print a single integer — the sought number of variants modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>l</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100, 1 ≤ <i>l</i> ≤ 3000</span>) — the number of different board types and the fence length, correspondingly. Next <span class="tex-span"><i>n</i></span> lines contain descriptions of board types: the <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the sizes of the board of the <span class="tex-span"><i>i</i></span>-th type. All numbers on the lines are separated by spaces.</p>

## Output

<p>Print a single integer — the sought number of variants modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
2 3
1 2
2 3

```




```input2
1 2
2 2

```




```input3
6 6
2 1
3 2
2 5
3 3
5 1
2 1

```




```output1
2

```




```output2
1

```




```output3
20

```



## Note

<p>In the first sample there are exactly two variants of arranging a beautiful fence of length 3: </p><ul> <li> As the first fence board use the board of the first type of length 1 and width 2. As the second board use board of the second type of length 2 and width 3. </li><li> Use one board of the second type after you turn it. That makes its length equal 3, and width — 2. </li></ul>
