## Description

<div><p>Company "Robots industries" produces robots for territory protection. Robots protect triangle territories — right isosceles triangles with catheti parallel to North-South and East-West directions.</p><p>Owner of some land buys and sets robots on his territory to protect it. From time to time, businessmen want to build offices on that land and want to know how many robots will guard it. You are to handle these queries. </p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>N</i></span> — width and height of the land, and integer <span class="tex-span"><i>Q</i></span> — number of queries to handle.</p><p>Next <span class="tex-span"><i>Q</i></span> lines contain queries you need to process.</p><p>Two types of queries: </p><ol> <li> <span class="tex-span">1</span> <span class="tex-span"><i>dir</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span"><i>len</i></span> — add a robot to protect a triangle. Depending on the value of <span class="tex-span"><i>dir</i></span>, the values of <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>len</i></span> represent a different triangle: <ul>  <li> <span class="tex-span"><i>dir</i> = 1</span>: Triangle is defined by the points <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i> + <i>len</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> + <i>len</i>)</span>  </li><li> <span class="tex-span"><i>dir</i> = 2</span>: Triangle is defined by the points <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i> + <i>len</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> - <i>len</i>)</span>  </li><li> <span class="tex-span"><i>dir</i> = 3</span>: Triangle is defined by the points <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i> - <i>len</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> + <i>len</i>)</span>  </li><li> <span class="tex-span"><i>dir</i> = 4</span>: Triangle is defined by the points <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i> - <i>len</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> - <i>len</i>)</span> </li></ul> </li><li> <span class="tex-span">2</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> — output how many robots guard this point (robot guards a point if the point is inside or on the border of its triangle) </li></ol><ul> <li> <span class="tex-span">1 ≤ <i>N</i> ≤ 5000</span> </li><li> <span class="tex-span">1 ≤ <i>Q</i> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">1 ≤ <i>dir</i> ≤ 4</span> </li><li> All points of triangles are within range <span class="tex-span">[1, <i>N</i>]</span> </li><li> All numbers are positive integers </li></ul></div><div class="output-specification"><p>For each second type query output how many robots guard this point. Each answer should be in a separate line.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>N</i></span> — width and height of the land, and integer <span class="tex-span"><i>Q</i></span> — number of queries to handle.</p><p>Next <span class="tex-span"><i>Q</i></span> lines contain queries you need to process.</p><p>Two types of queries: </p><ol> <li> <span class="tex-span">1</span> <span class="tex-span"><i>dir</i></span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> <span class="tex-span"><i>len</i></span> — add a robot to protect a triangle. Depending on the value of <span class="tex-span"><i>dir</i></span>, the values of <span class="tex-span"><i>x</i></span>, <span class="tex-span"><i>y</i></span> and <span class="tex-span"><i>len</i></span> represent a different triangle: <ul>  <li> <span class="tex-span"><i>dir</i> = 1</span>: Triangle is defined by the points <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i> + <i>len</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> + <i>len</i>)</span>  </li><li> <span class="tex-span"><i>dir</i> = 2</span>: Triangle is defined by the points <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i> + <i>len</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> - <i>len</i>)</span>  </li><li> <span class="tex-span"><i>dir</i> = 3</span>: Triangle is defined by the points <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i> - <i>len</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> + <i>len</i>)</span>  </li><li> <span class="tex-span"><i>dir</i> = 4</span>: Triangle is defined by the points <span class="tex-span">(<i>x</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i> - <i>len</i>, <i>y</i>)</span>, <span class="tex-span">(<i>x</i>, <i>y</i> - <i>len</i>)</span> </li></ul> </li><li> <span class="tex-span">2</span> <span class="tex-span"><i>x</i></span> <span class="tex-span"><i>y</i></span> — output how many robots guard this point (robot guards a point if the point is inside or on the border of its triangle) </li></ol><ul> <li> <span class="tex-span">1 ≤ <i>N</i> ≤ 5000</span> </li><li> <span class="tex-span">1 ≤ <i>Q</i> ≤ 10<sup class="upper-index">5</sup></span> </li><li> <span class="tex-span">1 ≤ <i>dir</i> ≤ 4</span> </li><li> All points of triangles are within range <span class="tex-span">[1, <i>N</i>]</span> </li><li> All numbers are positive integers </li></ul>

## Output

<p>For each second type query output how many robots guard this point. Each answer should be in a separate line.</p>





```input1
17 10
1 1 3 2 4
1 3 10 3 7
1 2 6 8 2
1 3 9 4 2
2 4 4
1 4 15 10 6
2 7 7
2 9 4
2 12 2
2 13 8

```




```output1
2
2
2
0
1

```


