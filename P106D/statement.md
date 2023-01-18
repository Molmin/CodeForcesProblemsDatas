## Description

<div><p>Our brave travelers reached an island where pirates had buried treasure. However as the ship was about to moor, the captain found out that some rat ate a piece of the treasure map.</p><p>The treasure map can be represented as a rectangle <span class="tex-span"><i>n</i> × <i>m</i></span> in size. Each cell stands for an islands' square (the square's side length equals to a mile). Some cells stand for the sea and they are impenetrable. All other cells are penetrable (i.e. available) and some of them contain local sights. For example, the large tree on the hills or the cave in the rocks.</p><p>Besides, the map also has a set of <span class="tex-span"><i>k</i></span> instructions. Each instruction is in the following form:</p><p>"Walk <span class="tex-span"><i>n</i></span> miles in the <span class="tex-span"><i>y</i></span> direction"</p><p>The possible directions are: north, south, east, and west. If you follow these instructions carefully (you should fulfill all of them, one by one) then you should reach exactly the place where treasures are buried. </p><p>Unfortunately the captain doesn't know the place where to start fulfilling the instructions — as that very piece of the map was lost. But the captain very well remembers that the place contained some local sight. Besides, the captain knows that the whole way goes through the island's penetrable squares.</p><p>The captain wants to know which sights are worth checking. He asks you to help him with that. </p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>).</p><p>Then follow <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> integers each — the island map's description. "<span class="tex-font-style-tt">#</span>" stands for the sea. It is guaranteed that all cells along the rectangle's perimeter are the sea. "<span class="tex-font-style-tt">.</span>" stands for a penetrable square without any sights and the sights are marked with uppercase Latin letters from "<span class="tex-font-style-tt">A</span>" to "<span class="tex-font-style-tt">Z</span>". Not all alphabet letters can be used. However, it is guaranteed that at least one of them is present on the map. All local sights are marked by different letters.</p><p>The next line contains number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>), after which <span class="tex-span"><i>k</i></span> lines follow. Each line describes an instruction. Each instruction possesses the form "<span class="tex-span"><i>dir</i></span> <span class="tex-span"><i>len</i></span>", where <span class="tex-span"><i>dir</i></span> stands for the direction and <span class="tex-span"><i>len</i></span> stands for the length of the way to walk. <span class="tex-span"><i>dir</i></span> can take values "<span class="tex-font-style-tt">N</span>", "<span class="tex-font-style-tt">S</span>", "<span class="tex-font-style-tt">W</span>" and "<span class="tex-font-style-tt">E</span>" for North, South, West and East correspondingly. At that, north is to the top, South is to the bottom, west is to the left and east is to the right. <span class="tex-span"><i>len</i></span> is an integer from <span class="tex-span">1</span> to <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>Print all local sights that satisfy to the instructions as a string without any separators in the alphabetical order. If no sight fits, print "<span class="tex-font-style-tt">no solution</span>" without the quotes.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">3 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>).</p><p>Then follow <span class="tex-span"><i>n</i></span> lines containing <span class="tex-span"><i>m</i></span> integers each — the island map's description. "<span class="tex-font-style-tt">#</span>" stands for the sea. It is guaranteed that all cells along the rectangle's perimeter are the sea. "<span class="tex-font-style-tt">.</span>" stands for a penetrable square without any sights and the sights are marked with uppercase Latin letters from "<span class="tex-font-style-tt">A</span>" to "<span class="tex-font-style-tt">Z</span>". Not all alphabet letters can be used. However, it is guaranteed that at least one of them is present on the map. All local sights are marked by different letters.</p><p>The next line contains number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>), after which <span class="tex-span"><i>k</i></span> lines follow. Each line describes an instruction. Each instruction possesses the form "<span class="tex-span"><i>dir</i></span> <span class="tex-span"><i>len</i></span>", where <span class="tex-span"><i>dir</i></span> stands for the direction and <span class="tex-span"><i>len</i></span> stands for the length of the way to walk. <span class="tex-span"><i>dir</i></span> can take values "<span class="tex-font-style-tt">N</span>", "<span class="tex-font-style-tt">S</span>", "<span class="tex-font-style-tt">W</span>" and "<span class="tex-font-style-tt">E</span>" for North, South, West and East correspondingly. At that, north is to the top, South is to the bottom, west is to the left and east is to the right. <span class="tex-span"><i>len</i></span> is an integer from <span class="tex-span">1</span> to <span class="tex-span">1000</span>.</p>

## Output

<p>Print all local sights that satisfy to the instructions as a string without any separators in the alphabetical order. If no sight fits, print "<span class="tex-font-style-tt">no solution</span>" without the quotes.</p>





```input1
6 10
##########
#K#..#####
#.#..##.##
#..L.#...#
###D###A.#
##########
4
N 2
S 1
E 1
W 2

```




```input2
3 4
####
#.A#
####
2
W 1
N 2

```




```output1
AD
```




```output2
no solution
```


