## Description

<div><p>Berland annual chess tournament is coming!</p><p>Organizers have gathered <span class="tex-span">2·<i>n</i></span> chess players who should be divided into two teams with <span class="tex-span"><i>n</i></span> people each. The first team is sponsored by BerOil and the second team is sponsored by BerMobile. Obviously, organizers should guarantee the win for the team of BerOil.</p><p>Thus, organizers should divide all <span class="tex-span">2·<i>n</i></span> players into two teams with <span class="tex-span"><i>n</i></span> people each in such a way that the first team always wins.</p><p>Every chess player has its rating <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>. It is known that chess player with the greater rating always wins the player with the lower rating. If their ratings are equal then any of the players can win.</p><p>After teams assignment there will come a drawing to form <span class="tex-span"><i>n</i></span> pairs of opponents: in each pair there is a player from the first team and a player from the second team. Every chess player should be in exactly one pair. Every pair plays once. The drawing is totally random.</p><p>Is it possible to divide all <span class="tex-span">2·<i>n</i></span> players into two teams with <span class="tex-span"><i>n</i></span> people each so that the player from the first team in every pair wins <span class="tex-font-style-bf">regardless</span> of the results of the drawing?</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>).</p><p>The second line contains <span class="tex-span">2·<i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index">2<i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p></div><div class="output-specification"><p>If it's possible to divide all <span class="tex-span">2·<i>n</i></span> players into two teams with <span class="tex-span"><i>n</i></span> people each so that the player from the first team in every pair wins regardless of the results of the drawing, then print <span class="tex-font-style-tt">"YES"</span>. Otherwise print <span class="tex-font-style-tt">"NO"</span>.</p></div>

## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>).</p><p>The second line contains <span class="tex-span">2·<i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index">2<i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>).</p>

## Output

<p>If it's possible to divide all <span class="tex-span">2·<i>n</i></span> players into two teams with <span class="tex-span"><i>n</i></span> people each so that the player from the first team in every pair wins regardless of the results of the drawing, then print <span class="tex-font-style-tt">"YES"</span>. Otherwise print <span class="tex-font-style-tt">"NO"</span>.</p>





```input1
2
1 3 2 4

```




```input2
1
3 3

```




```output1
YES

```




```output2
NO

```


