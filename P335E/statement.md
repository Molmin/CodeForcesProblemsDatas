## Description

<div><p>A number of skyscrapers have been built in a line. The number of skyscrapers was chosen uniformly at random between <span class="tex-span">2</span> and <span class="tex-span">314!</span> (314 factorial, a very large number). The height of each skyscraper was chosen randomly and independently, with height <span class="tex-span"><i>i</i></span> having probability <span class="tex-span">2<sup class="upper-index"> - <i>i</i></sup></span> for all positive integers <span class="tex-span"><i>i</i></span>. The floors of a skyscraper with height <span class="tex-span"><i>i</i></span> are numbered <span class="tex-span">0</span> through <span class="tex-span"><i>i</i> - 1</span>.</p><p>To speed up transit times, a number of zip lines were installed between skyscrapers. Specifically, there is a zip line connecting the <span class="tex-span"><i>i</i></span>-th floor of one skyscraper with the <span class="tex-span"><i>i</i></span>-th floor of another skyscraper if and only if there are no skyscrapers between them that have an <span class="tex-span"><i>i</i></span>-th floor.</p><p>Alice and Bob decide to count the number of skyscrapers.</p><p>Alice is thorough, and wants to know exactly how many skyscrapers there are. She begins at the leftmost skyscraper, with a counter at 1. She then moves to the right, one skyscraper at a time, adding 1 to her counter each time she moves. She continues until she reaches the rightmost skyscraper.</p><p>Bob is impatient, and wants to finish as fast as possible. He begins at the leftmost skyscraper, with a counter at 1. He moves from building to building using zip lines. At each stage Bob uses the highest available zip line to the right, but ignores floors with a height greater than <span class="tex-span"><i>h</i></span> due to fear of heights. When Bob uses a zip line, he travels too fast to count how many skyscrapers he passed. Instead, he just adds <span class="tex-span">2<sup class="upper-index"><i>i</i></sup></span> to his counter, where <span class="tex-span"><i>i</i></span> is the number of the floor he's currently on. He continues until he reaches the rightmost skyscraper.</p><p>Consider the following example. There are <span class="tex-span">6</span> buildings, with heights <span class="tex-span">1</span>, <span class="tex-span">4</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span>, <span class="tex-span">1</span>, <span class="tex-span">2</span> from left to right, and <span class="tex-span"><i>h</i> = 2</span>. Alice begins with her counter at <span class="tex-span">1</span> and then adds <span class="tex-span">1</span> five times for a result of <span class="tex-span">6</span>. Bob begins with his counter at <span class="tex-span">1</span>, then he adds <span class="tex-span">1</span>, <span class="tex-span">4</span>, <span class="tex-span">4</span>, and <span class="tex-span">2</span>, in order, for a result of <span class="tex-span">12</span>. Note that Bob ignores the highest zip line because of his fear of heights (<span class="tex-span"><i>h</i> = 2</span>).</p><center> <img class="tex-graphics" src="file://WdDInxjl.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Bob's counter is at the top of the image, and Alice's counter at the bottom. All zip lines are shown. Bob's path is shown by the green dashed line and Alice's by the pink dashed line. The floors of the skyscrapers are numbered, and the zip lines Bob uses are marked with the amount he adds to his counter.</p><p>When Alice and Bob reach the right-most skyscraper, they compare counters. You will be given either the value of Alice's counter or the value of Bob's counter, and must compute the expected value of the other's counter.</p></div><div class="input-specification"><p>The first line of input will be a name, either string "<span class="tex-font-style-tt">Alice</span>" or "<span class="tex-font-style-tt">Bob</span>". The second line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 30000</span>, <span class="tex-span">0 ≤ <i>h</i> ≤ 30</span>). If the name is "<span class="tex-font-style-tt">Alice</span>", then <span class="tex-span"><i>n</i></span> represents the value of Alice's counter when she reaches the rightmost skyscraper, otherwise <span class="tex-span"><i>n</i></span> represents the value of Bob's counter when he reaches the rightmost skyscraper; <span class="tex-span"><i>h</i></span> represents the highest floor number Bob is willing to use.</p></div><div class="output-specification"><p>Output a single real value giving the expected value of the Alice's counter if you were given Bob's counter, or Bob's counter if you were given Alice's counter. </p><p>You answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line of input will be a name, either string "<span class="tex-font-style-tt">Alice</span>" or "<span class="tex-font-style-tt">Bob</span>". The second line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 30000</span>, <span class="tex-span">0 ≤ <i>h</i> ≤ 30</span>). If the name is "<span class="tex-font-style-tt">Alice</span>", then <span class="tex-span"><i>n</i></span> represents the value of Alice's counter when she reaches the rightmost skyscraper, otherwise <span class="tex-span"><i>n</i></span> represents the value of Bob's counter when he reaches the rightmost skyscraper; <span class="tex-span"><i>h</i></span> represents the highest floor number Bob is willing to use.</p>

## Output

<p>Output a single real value giving the expected value of the Alice's counter if you were given Bob's counter, or Bob's counter if you were given Alice's counter. </p><p>You answer will be considered correct if its absolute or relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
Alice
3 1

```




```input2
Bob
2 30

```




```input3
Alice
2572 10

```




```output1
3.500000000

```




```output2
2

```




```output3
3439.031415943

```



## Note

<p>In the first example, Bob's counter has a 62.5% chance of being 3, a 25% chance of being 4, and a 12.5% chance of being 5.</p>
