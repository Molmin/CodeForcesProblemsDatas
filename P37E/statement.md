## Description

<div><p>Having unraveled the Berland Dictionary, the scientists managed to read the notes of the chroniclers of that time. For example, they learned how the chief of the ancient Berland tribe was chosen.</p><p>As soon as enough pretenders was picked, the following test took place among them: the chief of the tribe took a slab divided by horizontal and vertical stripes into identical squares (the slab consisted of <span class="tex-span"><i>N</i></span> lines and <span class="tex-span"><i>M</i></span> columns) and painted every square black or white. Then every pretender was given a slab of the same size but painted entirely white. Within a day a pretender could paint any side-linked set of the squares of the slab some color. The set is called linked if for any two squares belonging to the set there is a path belonging the set on which any two neighboring squares share a side. The aim of each pretender is to paint his slab in the exactly the same way as the chief’s slab is painted. The one who paints a slab like that first becomes the new chief.</p><p>Scientists found the slab painted by the ancient Berland tribe chief. Help them to determine the minimal amount of days needed to find a new chief if he had to paint his slab in the given way.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>N</i>, <i>M</i> ≤ 50</span>) — the number of lines and columns on the slab. The next <span class="tex-span"><i>N</i></span> lines contain <span class="tex-span"><i>M</i></span> symbols each — the final coloration of the slab. <span class="tex-span"><i>W</i></span> stands for the square that should be painted white and <span class="tex-span"><i>B</i></span> — for the square that should be painted black.</p></div><div class="output-specification"><p>In the single line output the minimal number of repaintings of side-linked areas needed to get the required coloration of the slab.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> (<span class="tex-span">1 ≤ <i>N</i>, <i>M</i> ≤ 50</span>) — the number of lines and columns on the slab. The next <span class="tex-span"><i>N</i></span> lines contain <span class="tex-span"><i>M</i></span> symbols each — the final coloration of the slab. <span class="tex-span"><i>W</i></span> stands for the square that should be painted white and <span class="tex-span"><i>B</i></span> — for the square that should be painted black.</p>

## Output

<p>In the single line output the minimal number of repaintings of side-linked areas needed to get the required coloration of the slab.</p>





```input1
3 3
WBW
BWB
WBW

```




```input2
2 3
BBB
BWB

```




```output1
2

```




```output2
1

```


