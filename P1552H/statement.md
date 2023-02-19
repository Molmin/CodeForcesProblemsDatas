## Description

<div><p>Let us call a point of the plane <span class="tex-font-style-it">admissible</span> if its coordinates are positive integers less than or equal to $200$.</p><p>There is an invisible rectangle such that: </p><ul> <li> its vertices are all admissible; </li><li> its sides are parallel to the coordinate axes; </li><li> its area is strictly positive. </li></ul> Your task is to guess the perimeter of this rectangle.<p>In order to guess it, you may ask at most $4$ queries. </p><p>In each query, you choose a nonempty subset of the admissible points and you are told how many of the chosen points are inside or on the boundary of the invisible rectangle.</p></div><div><h2>Interaction</h2><p>To ask a query (of the kind described in the statement), you shall print two lines:</p><ul> <li> In the first line print "<span class="tex-font-style-tt">? $k$</span>" (without the quotes) where $k$ ($k\ge 1$) is the number of chosen points. </li><li> In the second line print $2k$ integers $x_1,\, y_1,\, x_2,\, y_2,\, \dots,\, x_k,\, y_k$ ($1\le x_i,y_i\le 200$ for $i=1,2,\dots,k$) where $(x_1, y_1),\,(x_2, y_2),\,(x_3, y_3),\, \dots,\,(x_k, y_k)$ are the $k$ distinct admissible chosen points (the order of the points is not important). </li></ul> After this, you should read an integer — the number of chosen points that are inside or on the boundary of the invisible rectangle.<p>When you have identified the perimeter $p$ of the invisible rectangle, you must print "<span class="tex-font-style-tt">! $p$</span>" (without quotes) and terminate your program.</p><p>If you ask more than $4$ queries or if one of the queries is malformed, the interactor terminates immediately and your program receives verdict <span class="tex-font-style-tt">Wrong Answer</span>.</p><p><span class="tex-font-style-bf">The interactor may be adaptive</span> (i.e., the hidden rectangle may not be chosen before the beginning of the interaction).</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages. </li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack a solution, use the following format.</p><p>The input has only one line, containing the $4$ integers $x_0$, $y_0$, $x_1$, $y_1$ ($1\le x_0&lt;x_1\le 200$, $1\le y_0 &lt; y_1 \le 200$) — $(x_0,y_0)$ is the bottom-left vertex of the hidden rectangle and $(x_1, y_1)$ is the top-right vertex of the hidden rectangle.</p><p><span class="tex-font-style-bf">Note that for hacks the interaction won't be adaptive</span>.</p></div>





```input1
13 5 123 80
```




```input2
2 2 4 4
```




```input3
1 1 200 200
```




```output1

```




```output2

```




```output3

```



## Note

<p>The following is an example of interaction for the <span class="tex-font-style-bf">first sample</span> intended to show the format of the queries. $$ \begin{array}{l|l|l} \text{Query (contestant program)} &amp; \text{Answer (interactor)} &amp; \text{Explanation} \\ \hline \mathtt{?\ 4} &amp; &amp; \text{We choose the $4$ vertices of} \\ \mathtt{13\ 5\ 13\ 80\ 123\ 5\ 123\ 80} &amp; \mathtt{4} &amp;\text{the hidden rectangle.}\\ \hline \mathtt{?\ 5} &amp; &amp; \text{We choose $4$ points just outside the hidden}\\ \mathtt{100\ 4\ 100\ 81\ 12\ 40\ 124\ 40\ 50\ 50} &amp; \mathtt{1}&amp; \text{rectangle and also the point $(50,50)$.}\\ \hline \mathtt{?\ 2} &amp; &amp; \text{We choose the points $(1, 1)$} \\ \mathtt{200\ 200\ 1\ 1} &amp; \mathtt{0} &amp; \text{and $(200,200)$.}\\ \hline \mathtt{!\ 370} &amp; &amp; \text{This is the correct perimeter.} \end{array} $$</p><p>For the <span class="tex-font-style-bf">second sample</span>, a possible interaction is the following. $$ \begin{array}{l|l|l} \text{Query (contestant program)} &amp; \text{Answer (interactor)} &amp; \text{Explanation} \\ \hline \mathtt{?\ 4} &amp; &amp; \text{We choose the points $(3, 2)$, $(4, 1)$,} \\ \mathtt{3\ 2\ 4\ 1\ 5\ 2\ 4\ 3} &amp; 2 &amp; \text{$(5, 2)$ and $(4, 3)$.} \\ \hline \mathtt{?\ 7} &amp; &amp; \text{We choose the points $(1, 4)$, $(2, 4)$,} \\ \mathtt{1\ 4\ 2\ 4\ 1\ 5\ 2\ 5\ 5\ 5\ 5\ 6\ 6\ 5} &amp; 1 &amp; \text{$(1, 5)$, $(2, 5)$, $(5, 5)$, $(5, 6)$ and $(6, 5)$.} \\ \hline \mathtt{!\ 8} &amp; &amp; \text{This is the correct perimeter.} \end{array} $$ The situation is shown in the following picture:</p><center> <img class="tex-graphics" src="file://Xx0U6wsU.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The green points are the ones belonging to the first query, while the orange points are the ones belonging to the second query. One can see that there are exactly two rectangles consistent with the interactor's answers: </p><ul> <li> the rectangle of vertices $(2, 2)$ and $(4, 4)$, shown in red; </li><li> the rectangle of vertices $(4, 2)$ and $(5, 5)$, shown in blue. </li></ul> Since both of these rectangles have perimeter $8$, this is the final answer.
