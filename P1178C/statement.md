## Description

<div><p>Bob is decorating his kitchen, more precisely, the floor. He has found a prime candidate for the tiles he will use. They come in a simple form factor&nbsp;—&nbsp;a square tile that is diagonally split into white and black part as depicted in the figure below.</p><center> <img class="tex-graphics" src="file://1ZXdVczV.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The dimension of this tile is perfect for this kitchen, as he will need exactly $w \times h$ tiles without any scraps. That is, the width of the kitchen is $w$ tiles, and the height is $h$ tiles. As each tile can be rotated in one of four ways, he still needs to decide on how exactly he will tile the floor. There is a single aesthetic criterion that he wants to fulfil: two adjacent tiles must not share a colour on the edge&nbsp;—&nbsp;i.e. one of the tiles must have a white colour on the shared border, and the second one must be black.</p><center> <img class="tex-graphics" src="file://QBFQPcdb.png" style="max-width: 100.0%;max-height: 100.0%;">   <span class="tex-font-style-it">The picture on the left shows one valid tiling of a $3 \times 2$ kitchen. The picture on the right shows an invalid arrangement, as the bottom two tiles touch with their white parts.</span> </center><p>Find the number of possible tilings. As this number may be large, output its remainder when divided by $998244353$ (a prime number). </p></div><div class="input-specification"><p>The only line contains two space separated integers $w$, $h$&nbsp;($1 \leq w,h \leq 1\,000$)&nbsp;—&nbsp;the width and height of the kitchen, measured in tiles.</p></div><div class="output-specification"><p>Output a single integer $n$&nbsp;—&nbsp;the remainder of the number of tilings when divided by $998244353$.</p></div>

## Input

<p>The only line contains two space separated integers $w$, $h$&nbsp;($1 \leq w,h \leq 1\,000$)&nbsp;—&nbsp;the width and height of the kitchen, measured in tiles.</p>

## Output

<p>Output a single integer $n$&nbsp;—&nbsp;the remainder of the number of tilings when divided by $998244353$.</p>





```input1
2 2
```




```input2
2 4
```




```output1
16
```




```output2
64
```


