## Description

<div><p>It's Piegirl's birthday soon, and Pieguy has decided to buy her a bouquet of flowers and a basket of chocolates.</p><p>The flower shop has <span class="tex-span"><i>F</i></span> different types of flowers available. The <span class="tex-span"><i>i</i></span>-th type of flower always has exactly <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> petals. Pieguy has decided to buy a bouquet consisting of exactly <span class="tex-span"><i>N</i></span> flowers. He may buy the same type of flower multiple times. The <span class="tex-span"><i>N</i></span> flowers are then arranged into a bouquet. The position of the flowers within a bouquet matters. You can think of a bouquet as an ordered list of flower types.</p><p>The chocolate shop sells chocolates in boxes. There are <span class="tex-span"><i>B</i></span> different types of boxes available. The <span class="tex-span"><i>i</i></span>-th type of box contains <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> pieces of chocolate. Pieguy can buy any number of boxes, and can buy the same type of box multiple times. He will then place these boxes into a basket. The position of the boxes within the basket matters. You can think of the basket as an ordered list of box types.</p><p>Pieguy knows that Piegirl likes to pluck a petal from a flower before eating each piece of chocolate. He would like to ensure that she eats the last piece of chocolate from the last box just after plucking the last petal from the last flower. That is, the total number of petals on all the flowers in the bouquet should equal the total number of pieces of chocolate in all the boxes in the basket.</p><p>How many different bouquet+basket combinations can Pieguy buy? The answer may be very large, so compute it modulo <span class="tex-span">1000000007 = 10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line of input will contain integers <span class="tex-span"><i>F</i></span>, <span class="tex-span"><i>B</i></span>, and <span class="tex-span"><i>N</i></span> <span class="tex-span">(1 ≤ <i>F</i> ≤ 10, 1 ≤ <i>B</i> ≤ 100, 1 ≤ <i>N</i> ≤ 10<sup class="upper-index">18</sup>)</span>, the number of types of flowers, the number of types of boxes, and the number of flowers that must go into the bouquet, respectively.</p><p>The second line of input will contain <span class="tex-span"><i>F</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>F</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, the numbers of petals on each of the flower types.</p><p>The third line of input will contain <span class="tex-span"><i>B</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>B</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 250)</span>, the number of pieces of chocolate in each of the box types.</p></div><div class="output-specification"><p>Print the number of bouquet+basket combinations Pieguy can buy, modulo <span class="tex-span">1000000007 = 10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of input will contain integers <span class="tex-span"><i>F</i></span>, <span class="tex-span"><i>B</i></span>, and <span class="tex-span"><i>N</i></span> <span class="tex-span">(1 ≤ <i>F</i> ≤ 10, 1 ≤ <i>B</i> ≤ 100, 1 ≤ <i>N</i> ≤ 10<sup class="upper-index">18</sup>)</span>, the number of types of flowers, the number of types of boxes, and the number of flowers that must go into the bouquet, respectively.</p><p>The second line of input will contain <span class="tex-span"><i>F</i></span> integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>F</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, the numbers of petals on each of the flower types.</p><p>The third line of input will contain <span class="tex-span"><i>B</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>B</i></sub></span> <span class="tex-span">(1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 250)</span>, the number of pieces of chocolate in each of the box types.</p>

## Output

<p>Print the number of bouquet+basket combinations Pieguy can buy, modulo <span class="tex-span">1000000007 = 10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2 3 3
3 5
10 3 7

```




```input2
6 5 10
9 3 3 4 9 9
9 9 1 6 4

```




```output1
17

```




```output2
31415926

```



## Note

<p>In the first example, there is <span class="tex-span">1</span> way to make a bouquet with <span class="tex-span">9</span> petals <span class="tex-span">(3 + 3 + 3)</span>, and <span class="tex-span">1</span> way to make a basket with <span class="tex-span">9</span> pieces of chocolate <span class="tex-span">(3 + 3 + 3)</span>, for <span class="tex-span">1</span> possible combination. There are <span class="tex-span">3</span> ways to make a bouquet with <span class="tex-span">13</span> petals <span class="tex-span">(3 + 5 + 5, 5 + 3 + 5, 5 + 5 + 3)</span>, and <span class="tex-span">5</span> ways to make a basket with <span class="tex-span">13</span> pieces of chocolate <span class="tex-span">(3 + 10, 10 + 3, 3 + 3 + 7, 3 + 7 + 3, 7 + 3 + 3)</span>, for <span class="tex-span">15</span> more combinations. Finally there is <span class="tex-span">1</span> way to make a bouquet with <span class="tex-span">15</span> petals <span class="tex-span">(5 + 5 + 5)</span> and <span class="tex-span">1</span> way to make a basket with <span class="tex-span">15</span> pieces of chocolate <span class="tex-span">(3 + 3 + 3 + 3 + 3)</span>, for <span class="tex-span">1</span> more combination.</p><p>Note that it is possible for multiple types of flowers to have the same number of petals. Such types are still considered different. Similarly different types of boxes may contain the same number of pieces of chocolate, but are still considered different.</p>
