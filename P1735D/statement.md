## Description

<div><p>You like the card board game "Set". Each card contains $k$ features, each of which is equal to a value from the set $\{0, 1, 2\}$. The deck contains all possible variants of cards, that is, there are $3^k$ different cards in total.</p><p>A feature for three cards is called <span class="tex-font-style-it">good</span> if it is the same for these cards or pairwise distinct. Three cards are called a <span class="tex-font-style-it">set</span> if all $k$ features are good for them.</p><p>For example, the cards $(0, 0, 0)$, $(0, 2, 1)$, and $(0, 1, 2)$ form a set, but the cards $(0, 2, 2)$, $(2, 1, 2)$, and $(1, 2, 0)$ do not, as, for example, the last feature is not good.</p><p>A group of <span class="tex-font-style-bf">five</span> cards is called a <span class="tex-font-style-it">meta-set</span>, if there is strictly more than one set among them. How many meta-sets there are among given $n$ distinct cards?</p></div><div class="input-specification"><p>The first line of the input contains two integers $n$ and $k$ ($1 \le n \le 10^3$, $1 \le k \le 20$) — the number of cards on a table and the number of card features. The description of the cards follows in the next $n$ lines.</p><p>Each line describing a card contains $k$ integers $c_{i, 1}, c_{i, 2}, \ldots, c_{i, k}$ ($0 \le c_{i, j} \le 2$)&nbsp;— card features. It is guaranteed that all cards are distinct.</p></div><div class="output-specification"><p>Output one integer — the number of meta-sets.</p></div>

## Input

<p>The first line of the input contains two integers $n$ and $k$ ($1 \le n \le 10^3$, $1 \le k \le 20$) — the number of cards on a table and the number of card features. The description of the cards follows in the next $n$ lines.</p><p>Each line describing a card contains $k$ integers $c_{i, 1}, c_{i, 2}, \ldots, c_{i, k}$ ($0 \le c_{i, j} \le 2$)&nbsp;— card features. It is guaranteed that all cards are distinct.</p>

## Output

<p>Output one integer — the number of meta-sets.</p>





```input1
8 4
0 0 0 0
0 0 0 1
0 0 0 2
0 0 1 0
0 0 2 0
0 1 0 0
1 0 0 0
2 2 0 0
```




```input2
7 4
0 0 0 0
0 0 0 1
0 0 0 2
0 0 1 0
0 0 2 0
0 1 0 0
0 2 0 0
```




```input3
9 2
0 0
0 1
0 2
1 0
1 1
1 2
2 0
2 1
2 2
```




```input4
20 4
0 2 0 0
0 2 2 2
0 2 2 1
0 2 0 1
1 2 2 0
1 2 1 0
1 2 2 1
1 2 0 1
1 1 2 2
1 1 0 2
1 1 2 1
1 1 1 1
2 1 2 0
2 1 1 2
2 1 2 1
2 1 1 1
0 1 1 2
0 0 1 0
2 2 0 0
2 0 0 2
```




```output1
1
```




```output2
3
```




```output3
54
```




```output4
0
```



## Note

<p>Let's draw the cards indicating the first four features. The first feature will indicate the number of objects on a card: $1$, $2$, $3$. The second one is the color: red, green, purple. The third is the shape: oval, diamond, squiggle. The fourth is filling: open, striped, solid.</p><p>You can see the first three tests below. For the first two tests, the meta-sets are highlighted.</p><p>In the first test, the only meta-set is the five cards $(0000,\ 0001,\ 0002,\ 0010,\ 0020)$. The sets in it are the triples $(0000,\ 0001,\ 0002)$ and $(0000,\ 0010,\ 0020)$. Also, a set is the triple $(0100,\ 1000,\ 2200)$ which does not belong to any meta-set. </p><center> <img class="tex-graphics" src="file://aPNHw10c.png" style="max-width: 100.0%;max-height: 100.0%;" width="832px"> </center><p>In the second test, the following groups of five cards are meta-sets: $(0000,\ 0001,\ 0002,\ 0010,\ 0020)$, $(0000,\ 0001,\ 0002,\ 0100,\ 0200)$, $(0000,\ 0010,\ 0020,\ 0100,\ 0200)$. </p><center> <img class="tex-graphics" src="file://eXKp5wrE.png" style="max-width: 100.0%;max-height: 100.0%;" width="832px"> </center><p>In there third test, there are $54$ meta-sets. </p><center> <img class="tex-graphics" src="file://IHvhunWm.png" style="max-width: 100.0%;max-height: 100.0%;" width="832px"> </center>
