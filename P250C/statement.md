## Description

<div><p>A film festival is coming up in the city N. The festival will last for exactly <span class="tex-span"><i>n</i></span> days and each day will have a premiere of exactly one film. Each film has a genre — an integer from 1 to <span class="tex-span"><i>k</i></span>.</p><p>On the <span class="tex-span"><i>i</i></span>-th day the festival will show a movie of genre <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. We know that a movie of each of <span class="tex-span"><i>k</i></span> genres occurs in the festival programme at least once. In other words, each integer from 1 to <span class="tex-span"><i>k</i></span> occurs in the sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> at least once.</p><p>Valentine is a movie critic. He wants to watch some movies of the festival and then describe his impressions on his site.</p><p>As any creative person, Valentine is very susceptive. After he watched the movie of a certain genre, Valentine forms the <span class="tex-font-style-it">mood</span> he preserves until he watches the next movie. If the genre of the next movie is the same, it does not change Valentine's mood. If the genres are different, Valentine's mood changes according to the new genre and Valentine has a <span class="tex-font-style-it">stress</span>.</p><p>Valentine can't watch all <span class="tex-span"><i>n</i></span> movies, so he decided to exclude from his to-watch list movies of one of the genres. In other words, Valentine is going to choose exactly one of the <span class="tex-span"><i>k</i></span> genres and will skip all the movies of this genre. He is sure to visit other movies.</p><p>Valentine wants to choose such genre <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>x</i> ≤ <i>k</i></span>), that the total number of after-movie stresses (after all movies of genre <span class="tex-span"><i>x</i></span> are excluded) were minimum.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>n</i></span> is the number of movies and <span class="tex-span"><i>k</i></span> is the number of genres.</p><p>The second line of the input contains a sequence of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the genre of the <span class="tex-span"><i>i</i></span>-th movie. It is guaranteed that each number from 1 to <span class="tex-span"><i>k</i></span> occurs at least once in this sequence.</p></div><div class="output-specification"><p>Print a single number — the number of the genre (from 1 to <span class="tex-span"><i>k</i></span>) of the excluded films. If there are multiple answers, print the genre with the minimum number.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), where <span class="tex-span"><i>n</i></span> is the number of movies and <span class="tex-span"><i>k</i></span> is the number of genres.</p><p>The second line of the input contains a sequence of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>k</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the genre of the <span class="tex-span"><i>i</i></span>-th movie. It is guaranteed that each number from 1 to <span class="tex-span"><i>k</i></span> occurs at least once in this sequence.</p>

## Output

<p>Print a single number — the number of the genre (from 1 to <span class="tex-span"><i>k</i></span>) of the excluded films. If there are multiple answers, print the genre with the minimum number.</p>





```input1
10 3
1 1 2 3 2 3 3 1 1 3

```




```input2
7 3
3 1 3 2 3 1 2

```




```output1
3
```




```output2
1
```



## Note

<p>In the first sample if we exclude the movies of the 1st genre, the genres <span class="tex-span">2, 3, 2, 3, 3, 3</span> remain, that is 3 stresses; if we exclude the movies of the 2nd genre, the genres <span class="tex-span">1, 1, 3, 3, 3, 1, 1, 3</span> remain, that is 3 stresses; if we exclude the movies of the 3rd genre the genres <span class="tex-span">1, 1, 2, 2, 1, 1</span> remain, that is 2 stresses.</p><p>In the second sample whatever genre Valentine excludes, he will have exactly 3 stresses.</p>
