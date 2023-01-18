## Description

<div><p>A colored stripe is represented by a horizontal row of <span class="tex-span"><i>n</i></span> square cells, each cell is pained one of <span class="tex-span"><i>k</i></span> colors. Your task is to repaint the minimum number of cells so that no two neighbouring cells are of the same color. You can use any color from 1 to <span class="tex-span"><i>k</i></span> to repaint the cells.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>;&nbsp;2 ≤ <i>k</i> ≤ 26</span>). The second line contains <span class="tex-span"><i>n</i></span> uppercase English letters. Letter "<span class="tex-font-style-tt">A</span>" stands for the first color, letter "<span class="tex-font-style-tt">B</span>" stands for the second color and so on. The first <span class="tex-span"><i>k</i></span> English letters may be used. Each letter represents the color of the corresponding cell of the stripe.</p></div><div class="output-specification"><p>Print a single integer — the required minimum number of repaintings. In the second line print any possible variant of the repainted stripe.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup>;&nbsp;2 ≤ <i>k</i> ≤ 26</span>). The second line contains <span class="tex-span"><i>n</i></span> uppercase English letters. Letter "<span class="tex-font-style-tt">A</span>" stands for the first color, letter "<span class="tex-font-style-tt">B</span>" stands for the second color and so on. The first <span class="tex-span"><i>k</i></span> English letters may be used. Each letter represents the color of the corresponding cell of the stripe.</p>

## Output

<p>Print a single integer — the required minimum number of repaintings. In the second line print any possible variant of the repainted stripe.</p>





```input1
6 3
ABBACC

```




```input2
3 2
BBB

```




```output1
2
ABCACA

```




```output2
1
BAB

```


