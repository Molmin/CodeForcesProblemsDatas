## Description

<div><p>The competitors of Bubble Cup X gathered after the competition and discussed what is the best way to get to know the host country and its cities.</p><p>After exploring the map of Serbia for a while, the competitors came up with the following facts: the country has <span class="tex-span"><i>V</i></span> cities which are indexed with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>V</i></span>, and there are <span class="tex-span"><i>E</i></span> bi-directional roads that connect the cites. Each road has a weight (the time needed to cross that road). There are <span class="tex-span"><i>N</i></span> teams at the Bubble Cup and the competitors came up with the following plan: each of the <span class="tex-span"><i>N</i></span> teams will start their journey in one of the <span class="tex-span"><i>V</i></span> cities, and some of the teams share the starting position.</p><p>They want to find the shortest time <span class="tex-span"><i>T</i></span>, such that every team can move in these <span class="tex-span"><i>T</i></span> minutes, and the number of different cities they end up in is at least <span class="tex-span"><i>K</i></span> (because they will only get to know the cities they end up in). A team doesn't have to be on the move all the time, if they like it in a particular city, they can stay there and wait for the time to pass.</p><p>Please help the competitors to determine the shortest time <span class="tex-span"><i>T</i></span> so it's possible for them to end up in at least <span class="tex-span"><i>K</i></span> different cities or print <span class="tex-font-style-tt">-1</span> if that is impossible no matter how they move.</p><p>Note that there can exist multiple roads between some cities.</p></div><div class="input-specification"><p>The first line contains four integers: <span class="tex-span"><i>V</i></span>, <span class="tex-span"><i>E</i></span>, <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>K</i> (1 ≤  <i>V</i>  ≤  600,  1  ≤  <i>E</i>  ≤  20000,  1  ≤  <i>N</i>  ≤  <i>min</i>(<i>V</i>, 200),  1  ≤  <i>K</i>  ≤  <i>N</i>)</span>, number of cities, number of roads, number of teams and the smallest number of different cities they need to end up in, respectively.</p><p>The second line contains <span class="tex-span"><i>N</i></span> integers, the cities where the teams start their journey.</p><p>Next <span class="tex-span"><i>E</i></span> lines contain information about the roads in following format: <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub> <i>B</i><sub class="lower-index"><i>i</i></sub> <i>T</i><sub class="lower-index"><i>i</i></sub> (1 ≤ <i>A</i><sub class="lower-index"><i>i</i></sub>, <i>B</i><sub class="lower-index"><i>i</i></sub> ≤ <i>V</i>,  1 ≤ <i>T</i><sub class="lower-index"><i>i</i></sub> ≤ 10000)</span>, which means that there is a road connecting cities <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span>, and you need <span class="tex-span"><i>T</i><sub class="lower-index"><i>i</i></sub></span> minutes to cross that road.</p></div><div class="output-specification"><p>Output a single integer that represents the minimal time the teams can move for, such that they end up in at least <span class="tex-span"><i>K</i></span> different cities or output <span class="tex-font-style-tt">-1</span> if there is no solution.</p><p>If the solution exists, result will be no greater than <span class="tex-span">1731311</span>.</p></div>

## Input

<p>The first line contains four integers: <span class="tex-span"><i>V</i></span>, <span class="tex-span"><i>E</i></span>, <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>K</i> (1 ≤  <i>V</i>  ≤  600,  1  ≤  <i>E</i>  ≤  20000,  1  ≤  <i>N</i>  ≤  <i>min</i>(<i>V</i>, 200),  1  ≤  <i>K</i>  ≤  <i>N</i>)</span>, number of cities, number of roads, number of teams and the smallest number of different cities they need to end up in, respectively.</p><p>The second line contains <span class="tex-span"><i>N</i></span> integers, the cities where the teams start their journey.</p><p>Next <span class="tex-span"><i>E</i></span> lines contain information about the roads in following format: <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub> <i>B</i><sub class="lower-index"><i>i</i></sub> <i>T</i><sub class="lower-index"><i>i</i></sub> (1 ≤ <i>A</i><sub class="lower-index"><i>i</i></sub>, <i>B</i><sub class="lower-index"><i>i</i></sub> ≤ <i>V</i>,  1 ≤ <i>T</i><sub class="lower-index"><i>i</i></sub> ≤ 10000)</span>, which means that there is a road connecting cities <span class="tex-span"><i>A</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>B</i><sub class="lower-index"><i>i</i></sub></span>, and you need <span class="tex-span"><i>T</i><sub class="lower-index"><i>i</i></sub></span> minutes to cross that road.</p>

## Output

<p>Output a single integer that represents the minimal time the teams can move for, such that they end up in at least <span class="tex-span"><i>K</i></span> different cities or output <span class="tex-font-style-tt">-1</span> if there is no solution.</p><p>If the solution exists, result will be no greater than <span class="tex-span">1731311</span>.</p>





```input1
6 7 5 4
5 5 2 2 5
1 3 3
1 5 2
1 6 5
2 5 4
2 6 7
3 4 11
3 5 3

```




```output1
3
```



## Note

<p>Three teams start from city 5, and two teams start from city 2. If they agree to move for 3 minutes, one possible situation would be the following: Two teams in city 2, one team in city 5, one team in city 3 , and one team in city 1. And we see that there are four different cities the teams end their journey at.</p>
