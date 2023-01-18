## Description

<div><p><span class="tex-font-style-it">Piet Mondrian is an artist most famous for his minimalist works, consisting only of the four colors red, yellow, blue, and white. Most people attribute this to his style, but the truth is that his paint behaves in a very strange way where mixing two primary colors only produces another primary color!</span></p><center> <img class="tex-graphics" src="file://KrbJU9CS.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-style-it">A lesser known piece, entitled "Pretentious rectangles"</span> </center><p>A sequence of primary colors (red, yellow, blue) is mixed as follows. While there are at least two colors, look at the first two. If they are distinct, replace them with the missing color. If they are the same, remove them from the sequence. In the end, if there is one color, that is the resulting color. Otherwise, if the sequence is empty, we say the resulting color is white. Here are two example mixings:</p><center> <img class="tex-graphics" src="file://SU9HWPa1.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> &nbsp; <center> <img class="tex-graphics" src="file://pJUS2BV6.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Piet has a color palette with cells numbered from $1$ to $n$. Each cell contains a primary color or is empty. Piet is very secretive, and will not share his palette with you, so you do not know what colors belong to each cell.</p><p>However, he did perform $k$ operations. There are four kinds of operations: </p><ol> <li> In a <span class="tex-font-style-bf">mix</span> operation, Piet chooses a subset of cells and mixes their colors together in some order. The order is not necessarily by increasing indexes. He records the resulting color. Empty cells are skipped over, having no effect on the mixing process. The mixing does not change the color values stored in the cells. </li><li> In a <span class="tex-font-style-bf">RY</span> operation, Piet chooses a subset of cells. Any red cells in this subset become yellow, and any yellow cells in this subset become red. Blue and empty cells remain unchanged. </li><li> In a <span class="tex-font-style-bf">RB</span> operation, Piet chooses a subset of cells. Any red cells in this subset become blue, and any blue cells in this subset become red. Yellow and empty cells remain unchanged. </li><li> In a <span class="tex-font-style-bf">YB</span> operation, Piet chooses a subset of cells. Any yellow cells in this subset become blue, and any blue cells in this subset become yellow. Red and empty cells remain unchanged. </li></ol><p>Piet only tells you the list of operations he performs in chronological order, the indexes involved, and the resulting color of each mix operation. For each mix operation, you also know the order in which the cells are mixed. Given this information, determine the color of each cell in the initial palette. That is, you should find one possible state of the palette (before any operations were performed), or say that the described situation is impossible.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1\le n,k\le 1000$)&nbsp;— the number of cells in the palette and the number of operations, respectively.</p><p>The next $k$ lines describe the operations. The $i$-th line begins with the name of the $i$-th operation and an integer $m$ ($1\le m\le n$)&nbsp;— the number of indexes involved. Then follow $m$ integers $j_1,\ldots,j_m$ ($1\le j_i\le n$)&nbsp;— the indexes of the operation. It is guaranteed that all $j_i$ are distinct within an operation. If it is a mix operation, the indexes are listed in the order the colors are mixed, and the line also ends with a character representing the resulting color: "<span class="tex-font-style-tt">R</span>" for red, "<span class="tex-font-style-tt">Y</span>" for yellow, "<span class="tex-font-style-tt">B</span>" for blue, and "<span class="tex-font-style-tt">W</span>" for white.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">YES</span>" if a solution exists, or "<span class="tex-font-style-tt">NO</span>" otherwise. You can print each character in any case (upper or lower).</p><p>If the answer is "<span class="tex-font-style-tt">YES</span>", on the next line output a string of length $n$, consisting of characters "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">Y</span>", "<span class="tex-font-style-tt">B</span>", and "<span class="tex-font-style-tt">.</span>", representing the paint colors in the $n$ cells of the initial palette (red, yellow, blue, and empty, respectively). If there are multiple solutions, print any. You can print each character in any case (upper or lower).</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1\le n,k\le 1000$)&nbsp;— the number of cells in the palette and the number of operations, respectively.</p><p>The next $k$ lines describe the operations. The $i$-th line begins with the name of the $i$-th operation and an integer $m$ ($1\le m\le n$)&nbsp;— the number of indexes involved. Then follow $m$ integers $j_1,\ldots,j_m$ ($1\le j_i\le n$)&nbsp;— the indexes of the operation. It is guaranteed that all $j_i$ are distinct within an operation. If it is a mix operation, the indexes are listed in the order the colors are mixed, and the line also ends with a character representing the resulting color: "<span class="tex-font-style-tt">R</span>" for red, "<span class="tex-font-style-tt">Y</span>" for yellow, "<span class="tex-font-style-tt">B</span>" for blue, and "<span class="tex-font-style-tt">W</span>" for white.</p>

## Output

<p>Output "<span class="tex-font-style-tt">YES</span>" if a solution exists, or "<span class="tex-font-style-tt">NO</span>" otherwise. You can print each character in any case (upper or lower).</p><p>If the answer is "<span class="tex-font-style-tt">YES</span>", on the next line output a string of length $n$, consisting of characters "<span class="tex-font-style-tt">R</span>", "<span class="tex-font-style-tt">Y</span>", "<span class="tex-font-style-tt">B</span>", and "<span class="tex-font-style-tt">.</span>", representing the paint colors in the $n$ cells of the initial palette (red, yellow, blue, and empty, respectively). If there are multiple solutions, print any. You can print each character in any case (upper or lower).</p>





```input1
3 2
mix 2 2 1 R
mix 2 1 3 Y
```




```input2
2 3
mix 1 2 Y
RB 1 2
mix 1 2 W
```




```input3
1 3
RY 1 1
YB 1 1
mix 1 1 B
```




```input4
3 8
mix 2 1 2 R
mix 2 1 3 Y
RY 2 2 3
RB 3 1 2 3
YB 3 1 2 3
mix 1 1 W
mix 1 2 B
mix 1 3 Y
```




```output1
YES
YB.
```




```output2
NO
```




```output3
YES
R
```




```output4
YES
.RY
```



## Note

<p>For the first test case, the answer "<span class="tex-font-style-tt">YB.</span>" is consistent with both mixings. The first mixing "<span class="tex-font-style-tt">BY</span>" results in red, while the second mixing "<span class="tex-font-style-tt">Y</span>" results in yellow (the empty cell is ignored). Other valid solutions include "<span class="tex-font-style-tt">BYR</span>" and "<span class="tex-font-style-tt">.RY</span>".</p><p>For the second test case, we can show that no solution exists.</p><p>For the third test case, the answer "<span class="tex-font-style-tt">R</span>" is consistent with all operations. In the first two operations it changes to "<span class="tex-font-style-tt">Y</span>", then "<span class="tex-font-style-tt">B</span>". In the final operation, the mixing "<span class="tex-font-style-tt">B</span>" results in blue.</p><p>For the fourth test case, the answer "<span class="tex-font-style-tt">.RY</span>" is consistent with all operations. The first two mixings are "<span class="tex-font-style-tt">R</span>" and "<span class="tex-font-style-tt">Y</span>", resulting in red and yellow, respectively. During the next three operations, the palette changes to "<span class="tex-font-style-tt">.YR</span>", then "<span class="tex-font-style-tt">.YB</span>", then "<span class="tex-font-style-tt">.BY</span>". The final three mixings agree with this palette.</p>
