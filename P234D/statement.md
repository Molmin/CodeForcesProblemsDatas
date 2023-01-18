## Description

<div><p>Overall there are <span class="tex-span"><i>m</i></span> actors in Berland. Each actor has a personal identifier — an integer from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> (distinct actors have distinct identifiers). Vasya likes to watch Berland movies with Berland actors, and he has <span class="tex-span"><i>k</i></span> favorite actors. He watched the movie trailers for the next month and wrote the following information for every movie: the movie title, the number of actors who starred in it, and the identifiers of these actors. Besides, he managed to copy the movie titles and how many actors starred there, but he didn't manage to write down the identifiers of some actors. Vasya looks at his records and wonders which movies may be his favourite, and which ones may not be. Once Vasya learns the exact cast of all movies, his favorite movies will be determined as follows: a movie becomes favorite movie, if no other movie from Vasya's list has more favorite actors.</p><p>Help the boy to determine the following for each movie:</p><ul><li> whether it surely will be his favourite movie;</li><li> whether it surely won't be his favourite movie; </li><li> can either be favourite or not.</li></ul></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100, 1 ≤ <i>k</i> ≤ <i>m</i></span>) — the number of actors in Berland and the number of Vasya's favourite actors. </p><p>The second line contains <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) — the identifiers of Vasya's favourite actors.</p><p>The third line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of movies in Vasya's list.</p><p>Then follow <span class="tex-span"><i>n</i></span> blocks of lines, each block contains a movie's description. The <span class="tex-span"><i>i</i></span>-th movie's description contains three lines: </p><ul> <li> the first line contains string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> consists of lowercase English letters and can have the length of from <span class="tex-span">1</span> to <span class="tex-span">10</span> characters, inclusive) — the movie's title, </li><li> the second line contains a non-negative integer <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) — the number of actors who starred in this movie,</li><li> the third line has <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>m</i></span>) — the identifiers of the actors who star in this movie. If <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span>, than Vasya doesn't remember the identifier of the <span class="tex-span"><i>j</i></span>-th actor. It is guaranteed that the list of actors for a movie doesn't contain the same actors. </li></ul><p>All movies have distinct names. The numbers on the lines are separated by single spaces.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines in the output. In the <span class="tex-span"><i>i</i></span>-th line print: </p><ul> <li> 0, if the <span class="tex-span"><i>i</i></span>-th movie will surely be the favourite; </li><li> 1, if the <span class="tex-span"><i>i</i></span>-th movie won't surely be the favourite; </li><li> 2, if the <span class="tex-span"><i>i</i></span>-th movie can either be favourite, or not favourite. </li></ul></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 100, 1 ≤ <i>k</i> ≤ <i>m</i></span>) — the number of actors in Berland and the number of Vasya's favourite actors. </p><p>The second line contains <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) — the identifiers of Vasya's favourite actors.</p><p>The third line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of movies in Vasya's list.</p><p>Then follow <span class="tex-span"><i>n</i></span> blocks of lines, each block contains a movie's description. The <span class="tex-span"><i>i</i></span>-th movie's description contains three lines: </p><ul> <li> the first line contains string <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> consists of lowercase English letters and can have the length of from <span class="tex-span">1</span> to <span class="tex-span">10</span> characters, inclusive) — the movie's title, </li><li> the second line contains a non-negative integer <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) — the number of actors who starred in this movie,</li><li> the third line has <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>m</i></span>) — the identifiers of the actors who star in this movie. If <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> = 0</span>, than Vasya doesn't remember the identifier of the <span class="tex-span"><i>j</i></span>-th actor. It is guaranteed that the list of actors for a movie doesn't contain the same actors. </li></ul><p>All movies have distinct names. The numbers on the lines are separated by single spaces.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> lines in the output. In the <span class="tex-span"><i>i</i></span>-th line print: </p><ul> <li> 0, if the <span class="tex-span"><i>i</i></span>-th movie will surely be the favourite; </li><li> 1, if the <span class="tex-span"><i>i</i></span>-th movie won't surely be the favourite; </li><li> 2, if the <span class="tex-span"><i>i</i></span>-th movie can either be favourite, or not favourite. </li></ul>





```input1
5 3
1 2 3
6
firstfilm
3
0 0 0
secondfilm
4
0 0 4 5
thirdfilm
1
2
fourthfilm
1
5
fifthfilm
1
4
sixthfilm
2
1 0

```




```input2
5 3
1 3 5
4
jumanji
3
0 0 0
theeagle
5
1 2 3 4 0
matrix
3
2 4 0
sourcecode
2
2 4

```




```output1
2
2
1
1
1
2

```




```output2
2
0
1
1

```



## Note

<p>Note to the second sample: </p><ul> <li> Movie <span class="tex-font-style-tt">jumanji</span> can theoretically have from 1 to 3 Vasya's favourite actors. </li><li> Movie <span class="tex-font-style-tt">theeagle</span> has all three favourite actors, as the actor Vasya failed to remember, can only have identifier 5. </li><li> Movie <span class="tex-font-style-tt">matrix</span> can have exactly one favourite actor. </li><li> Movie <span class="tex-font-style-tt">sourcecode</span> doesn't have any favourite actors. </li></ul><p>Thus, movie <span class="tex-font-style-tt">theeagle</span> will surely be favourite, movies <span class="tex-font-style-tt">matrix</span> and <span class="tex-font-style-tt">sourcecode</span> won't surely be favourite, and movie <span class="tex-font-style-tt">jumanji</span> can be either favourite (if it has all three favourite actors), or not favourite.</p>
