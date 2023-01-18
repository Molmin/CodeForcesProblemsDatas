## Description

<div><p>Once upon a time, when the world was more beautiful, the sun shone brighter, the grass was greener and the sausages tasted better Arlandia was the most powerful country. And its capital was the place where our hero DravDe worked. He couldn’t program or make up problems (in fact, few people saw a computer those days) but he was nevertheless happy. He worked in a warehouse where a magical but non-alcoholic drink Ogudar-Olok was kept. We won’t describe his work in detail and take a better look at a simplified version of the warehouse.</p><p>The warehouse has one set of shelving. It has <span class="tex-span"><i>n</i></span> shelves, each of which is divided into <span class="tex-span"><i>m</i></span> sections. The shelves are numbered from top to bottom starting from <span class="tex-span">1</span> and the sections of each shelf are numbered from left to right also starting from <span class="tex-span">1</span>. Each section can contain exactly one box of the drink, and try as he might, DravDe can never put a box in a section that already has one. In the course of his work DravDe frequently notices that he has to put a box in a filled section. In that case his solution is simple. DravDe ignores that section and looks at the next one to the right. If it is empty, he puts the box there. Otherwise he keeps looking for the first empty section to the right. If no empty section is found by the end of the shelf, he looks at the shelf which is under it, then the next one, etc. Also each time he looks at a new shelf he starts from the shelf’s beginning. If DravDe still can’t find an empty section for the box, he immediately drinks it all up and throws the empty bottles away not to be caught.</p><p>After one great party with a lot of Ogudar-Olok drunk DravDe asked you to help him. Unlike him, you can program and therefore modeling the process of counting the boxes in the warehouse will be easy work for you.</p><p>The process of counting contains two types of query messages: </p><ul> <li> «<span class="tex-font-style-bf"><span class="tex-font-style-tt">+1 x y id</span></span>» (where <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> are integers, <span class="tex-span">1 ≤ <i>x</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>y</i> ≤ <i>m</i></span>, and <span class="tex-span"><i>id</i></span> is a string of lower case Latin letters — from <span class="tex-span">1</span> to <span class="tex-span">10</span> characters long). That query means that the warehouse got a box identified as <span class="tex-span"><i>id</i></span>, which should be put in the section <span class="tex-span"><i>y</i></span> on the shelf <span class="tex-span"><i>x</i></span>. If the section is full, use the rules described above. It is guaranteed that every moment of the process the identifiers of all the boxes in the warehouse are different. You don’t have to answer this query. </li><li> «<span class="tex-font-style-bf"><span class="tex-font-style-tt">-1 id</span></span>» (where <span class="tex-span"><i>id</i></span> is a string of lower case Latin letters — from <span class="tex-span">1</span> to <span class="tex-span">10</span> characters long). That query means that a box identified as <span class="tex-span"><i>id</i></span> is removed from the warehouse. You have to answer this query (see output format). </li></ul></div><div class="input-specification"><p>The first input line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 30</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2000</span>) — the height, the width of shelving and the amount of the operations in the warehouse that you need to analyze. In the following <span class="tex-span"><i>k</i></span> lines the queries are given in the order of appearance in the format described above.</p></div><div class="output-specification"><p>For each query of the «<span class="tex-font-style-bf"><span class="tex-font-style-tt">-1 id</span></span>» type output two numbers in a separate line — index of the shelf and index of the section where the box with this identifier lay. If there was no such box in the warehouse when the query was made, output «<span class="tex-font-style-bf"><span class="tex-font-style-tt">-1 -1</span></span>» without quotes.</p></div>

## Input

<p>The first input line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 30</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 2000</span>) — the height, the width of shelving and the amount of the operations in the warehouse that you need to analyze. In the following <span class="tex-span"><i>k</i></span> lines the queries are given in the order of appearance in the format described above.</p>

## Output

<p>For each query of the «<span class="tex-font-style-bf"><span class="tex-font-style-tt">-1 id</span></span>» type output two numbers in a separate line — index of the shelf and index of the section where the box with this identifier lay. If there was no such box in the warehouse when the query was made, output «<span class="tex-font-style-bf"><span class="tex-font-style-tt">-1 -1</span></span>» without quotes.</p>





```input1
2 2 9
+1 1 1 cola
+1 1 1 fanta
+1 1 1 sevenup
+1 1 1 whitekey
-1 cola
-1 fanta
-1 sevenup
-1 whitekey
-1 cola

```




```input2
2 2 8
+1 1 1 cola
-1 cola
+1 1 1 fanta
-1 fanta
+1 1 1 sevenup
-1 sevenup
+1 1 1 whitekey
-1 whitekey

```




```output1
1 1
1 2
2 1
2 2
-1 -1

```




```output2
1 1
1 1
1 1
1 1

```


