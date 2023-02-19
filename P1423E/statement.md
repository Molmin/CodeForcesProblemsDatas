## Description

<div><p>After making a strategic plan with carriers for expansion of mobile network throughout the whole country, the government decided to cover rural areas with the last generation of 5G network.</p><p>Since 5G antenna towers will be built in the area of mainly private properties, the government needs an easy way to find information about landowners for each <span class="tex-font-style-bf">property</span> partially or fully contained in the planned building area. </p><p>The planned building area is represented as a rectangle with sides $width$ and $height$.</p><p>Every 5G antenna tower occupies a <span class="tex-font-style-bf">circle</span> with a center in $(x,y)$ and radius $r$. </p><p>There is a database of Geodetic Institute containing information about each property. Each property is defined with its <span class="tex-font-style-bf">identification number</span> and <span class="tex-font-style-bf">polygon</span> represented as an array of $(x,y)$ points in the counter-clockwise direction. </p><p>Your task is to build an IT system which can handle queries of type $(x, y, r)$ in which $(x,y)$ represents a circle center, while $r$ represents its radius. The IT system should return the <span class="tex-font-style-bf">total area</span> of properties that need to be acquired for the building of a tower so that the government can estimate the price. Furthermore, the system should return a list of <span class="tex-font-style-bf">identification numbers</span> of these properties (so that the owners can be contacted for land acquisition).</p><p>A property needs to be acquired if the circle of the antenna tower is intersecting or touching it. </p></div><div class="input-specification"><p>The first line contains the size of the building area as double values $width$, $height$, and an integer $n$ — the number of properties in the database. </p><p>Each of the next $n$ lines contains the description of a single property in the form of an integer number $v$ ($3 \le v \le 40$) — the number of points that define a property, as well as $2*v$ double numbers — the coordinates $(x,y)$ of each property point. Line $i$ ($0 \le i \le n-1$) contains the information for property with id $i$.</p><p>The next line contains an integer $q$ — the number of queries. </p><p>Each of the next $q$ lines contains double values $x$, $y$, $r$ — the coordinates of an antenna circle center $(x, y)$ and its radius $r$.</p><p>$1 \le n * q \le 10^6$</p></div><div class="output-specification"><p>For each of the $q$ queries, your program should output a line containing the total area of all the properties that need to be acquired, an integer representing the number of such properties, as well as the list of ids of these properties (separated by blank characters, arbitrary order).</p></div>

## Input

<p>The first line contains the size of the building area as double values $width$, $height$, and an integer $n$ — the number of properties in the database. </p><p>Each of the next $n$ lines contains the description of a single property in the form of an integer number $v$ ($3 \le v \le 40$) — the number of points that define a property, as well as $2*v$ double numbers — the coordinates $(x,y)$ of each property point. Line $i$ ($0 \le i \le n-1$) contains the information for property with id $i$.</p><p>The next line contains an integer $q$ — the number of queries. </p><p>Each of the next $q$ lines contains double values $x$, $y$, $r$ — the coordinates of an antenna circle center $(x, y)$ and its radius $r$.</p><p>$1 \le n * q \le 10^6$</p>

## Output

<p>For each of the $q$ queries, your program should output a line containing the total area of all the properties that need to be acquired, an integer representing the number of such properties, as well as the list of ids of these properties (separated by blank characters, arbitrary order).</p>





```input1
10 10 3
4 2 2 3 2 3 3 2 3
3 3.5 2 4.5 2 4.5 3
4 7 8 7.5 8.5 8 8 7.5 9
5
2 3.5 0.5
3.3 2 0.4
5 2.5 0.5
7.5 8.5 0.5
3 7 0.5
```




```output1
1.000000 1 0 
1.500000 2 0 1 
0.500000 1 1 
0.250000 1 2 
0.000000 0
```



## Note

<p>You can assume that the land not covered with properties (polygons) is under the government's ownership and therefore doesn't need to be acquired. Properties do not intersect with each other.</p><p>Precision being used for solution checking is $10^{-4}$.</p>
