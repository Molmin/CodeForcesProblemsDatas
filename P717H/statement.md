## Description

<div><p>Welcome to the world of Pokermon, yellow little mouse-like creatures, who absolutely love playing poker! </p><p>Yeah, right… </p><p>In the ensuing Pokermon League, there are <span class="tex-span"><i>n</i></span> registered Pokermon trainers, and <span class="tex-span"><i>t</i></span> existing trainer teams each of which belongs to one of two conferences. Since there is a lot of jealousy between trainers, there are <span class="tex-span"><i>e</i></span> pairs of trainers who hate each other. Their hate is mutual, there are no identical pairs among these, and no trainer hates himself (the world of Pokermon is a joyful place!). Each trainer has a wish-list of length <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> of teams he’d like to join.</p><p>Your task is to divide players into teams and the teams into two conferences, so that: </p><ul>  <li> each trainer belongs to exactly one team;  </li><li> no team is in both conferences;  </li><li> total hate between conferences is at least <span class="tex-span"><i>e</i> / 2</span>;  </li><li> every trainer is in a team from his wish-list. </li></ul><p>Total hate between conferences is calculated as the number of pairs of trainers from teams from different conferences who hate each other. </p></div><div class="input-specification"><p>The first line of the input contains two integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 50 000</span>) and <span class="tex-span"><i>e</i></span> (<span class="tex-span">2 ≤ <i>e</i> ≤ 100 000</span>)&nbsp;— the total number of Pokermon trainers and the number of pairs of trainers who hate each other.</p><p>Pokermon trainers are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Next <span class="tex-span"><i>e</i></span> lines contain two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>) indicating that Pokermon trainers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> hate each other. Next <span class="tex-span">2<i>n</i></span> lines are in a following format. Starting with Pokermon trainer <span class="tex-span">1</span>, for each trainer in consecutive order: first number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">16 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 20</span>)&nbsp;— a size of Pokermon trainers wish list, then <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> positive integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>T</i></span>), providing the teams the <span class="tex-span"><i>i</i></span>-th trainer would like to be on.</p><p>Each trainers wish list will contain each team no more than once. Teams on the wish lists are numbered in such a way that the set of all teams that appear on at least <span class="tex-span">1</span> wish list is set of consecutive positive integers <span class="tex-span">{1, 2, 3, …, <i>T</i>}</span>. Here <span class="tex-span"><i>T</i></span> might be up to <span class="tex-span">1 000 000</span>.</p></div><div class="output-specification"><p>Print two lines. The first line should contain <span class="tex-span"><i>n</i></span> numbers, specifying for each trainer the team he is in.</p><p>The second line should contain <span class="tex-span"><i>T</i></span> numbers, specifying the conference for each team (<span class="tex-span">1</span> or <span class="tex-span">2</span>).</p></div>

## Input

<p>The first line of the input contains two integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">4 ≤ <i>n</i> ≤ 50 000</span>) and <span class="tex-span"><i>e</i></span> (<span class="tex-span">2 ≤ <i>e</i> ≤ 100 000</span>)&nbsp;— the total number of Pokermon trainers and the number of pairs of trainers who hate each other.</p><p>Pokermon trainers are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Next <span class="tex-span"><i>e</i></span> lines contain two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>) indicating that Pokermon trainers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> hate each other. Next <span class="tex-span">2<i>n</i></span> lines are in a following format. Starting with Pokermon trainer <span class="tex-span">1</span>, for each trainer in consecutive order: first number <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">16 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 20</span>)&nbsp;— a size of Pokermon trainers wish list, then <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> positive integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>T</i></span>), providing the teams the <span class="tex-span"><i>i</i></span>-th trainer would like to be on.</p><p>Each trainers wish list will contain each team no more than once. Teams on the wish lists are numbered in such a way that the set of all teams that appear on at least <span class="tex-span">1</span> wish list is set of consecutive positive integers <span class="tex-span">{1, 2, 3, …, <i>T</i>}</span>. Here <span class="tex-span"><i>T</i></span> might be up to <span class="tex-span">1 000 000</span>.</p>

## Output

<p>Print two lines. The first line should contain <span class="tex-span"><i>n</i></span> numbers, specifying for each trainer the team he is in.</p><p>The second line should contain <span class="tex-span"><i>T</i></span> numbers, specifying the conference for each team (<span class="tex-span">1</span> or <span class="tex-span">2</span>).</p>





```input1
4 3
1 2
2 3
4 1
16
1 2 3 4 5 6 7 8 9 10 11 12 13 14 16 15
16
2 3 4 5 6 7 8 9 10 11 12 13 14 15 17 18
16
2 3 4 5 6 7 8 9 10 11 12 13 14 15 18 19
16
1 2 3 4 5 6 7 8 9 10 11 12 13 14 16 19

```




```output1
16 15 19 14 
2 2 2 1 1 1 2 1 1 2 1 1 1 2 2 1 1 1 1
```


