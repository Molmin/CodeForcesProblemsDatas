## Description

<div><p>Student Vasya came to study in Berland State University from the country, so he is living in a dormitory. A semester has <span class="tex-span"><i>n</i></span> days, and in each of those days his parents send him some food. In the morning of the <span class="tex-span"><i>i</i></span>-th day he receives <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> kilograms of food that can be eaten on that day and on the next one (then the food goes bad and becomes unfit for consumption).</p><p>Every day Vasya eats <span class="tex-span"><i>v</i></span> kilograms of food. It is known that Vasya's parents do not allow him to starve, so there always is enough food for Vasya. Vasya has <span class="tex-span"><i>m</i></span> friends who sometimes live with him. Let's index the friends from 1 to <span class="tex-span"><i>m</i></span>. Friend number <span class="tex-span"><i>j</i></span> lives with Vasya from day <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub></span> to day <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span>, inclusive. Also, the <span class="tex-span"><i>j</i></span>-th friend requires <span class="tex-span"><i>f</i><sub class="lower-index"><i>j</i></sub></span> kilograms of food per day. Usually Vasya's friends eat in the canteen, but sometimes generous Vasya feeds some of them. Every day Vasya can feed some friends who live with him this day (or may feed nobody).</p><p>Every time Vasya feeds his friend, he gives him as much food as the friend needs for the day, and Vasya's popularity rating at the University increases by one. Vasya cannot feed the same friend multiple times in one day. In addition, he knows that eating habits must be regular, so he always eats <span class="tex-span"><i>v</i></span> kilograms of food per day.</p><p>Vasya wants so choose whom he will feed each day of the semester to make his rating as high as possible. Originally Vasya's rating is 0 because he is a freshman.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>v</i> ≤ 400</span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 400</span>), separated by single spaces. Value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> means that in the morning of the <span class="tex-span"><i>i</i></span>-th day <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> kilograms of food come, the food is good for eating on day <span class="tex-span"><i>i</i></span> and/or on day <span class="tex-span"><i>i</i> + 1</span> (then the food goes bad). It is guaranteed that if Vasya doesn't feed anyone, there is a way for him to eat so as to consume <span class="tex-span"><i>v</i></span> kilograms of food every day.</p><p>The third line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 400</span>). Each of the following <span class="tex-span"><i>m</i></span> lines describes one Vasya's friend: the <span class="tex-span"><i>j</i></span>-th of these lines contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub>, <i>f</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>, 1 ≤ <i>f</i><sub class="lower-index"><i>j</i></sub> ≤ 400</span>), separated by single spaces.</p></div><div class="output-specification"><p>In the first line print the highest rating Vasya can reach. In the next <span class="tex-span"><i>n</i></span> lines print, which friends Vasya needs to feed on each day. In the <span class="tex-span"><i>i</i></span>-th of these lines first print the number of friends to feed on the <span class="tex-span"><i>i</i></span>-th day, and then list the indexes of these friends. Print the friends in these lists in any order. If there are multiple optimal solutions, print any of them.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>v</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>v</i> ≤ 400</span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 400</span>), separated by single spaces. Value <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> means that in the morning of the <span class="tex-span"><i>i</i></span>-th day <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> kilograms of food come, the food is good for eating on day <span class="tex-span"><i>i</i></span> and/or on day <span class="tex-span"><i>i</i> + 1</span> (then the food goes bad). It is guaranteed that if Vasya doesn't feed anyone, there is a way for him to eat so as to consume <span class="tex-span"><i>v</i></span> kilograms of food every day.</p><p>The third line contains integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 400</span>). Each of the following <span class="tex-span"><i>m</i></span> lines describes one Vasya's friend: the <span class="tex-span"><i>j</i></span>-th of these lines contains three integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub>, <i>f</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i>, 1 ≤ <i>f</i><sub class="lower-index"><i>j</i></sub> ≤ 400</span>), separated by single spaces.</p>

## Output

<p>In the first line print the highest rating Vasya can reach. In the next <span class="tex-span"><i>n</i></span> lines print, which friends Vasya needs to feed on each day. In the <span class="tex-span"><i>i</i></span>-th of these lines first print the number of friends to feed on the <span class="tex-span"><i>i</i></span>-th day, and then list the indexes of these friends. Print the friends in these lists in any order. If there are multiple optimal solutions, print any of them.</p>





```input1
4 1
3 2 5 4
3
1 3 2
1 4 1
3 4 2

```




```output1
7
1 2
1 2
3 2 1 3
2 2 3

```


