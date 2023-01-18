## Description

<div><p>In Berland, there is the national holiday coming — the Flag Day. In the honor of this event the president of the country decided to make a big dance party and asked your agency to organize it. He has several conditions:</p><ul> <li> overall, there must be <span class="tex-span"><i>m</i></span> dances;</li><li> exactly three people must take part in each dance;</li><li> each dance must have one dancer in white clothes, one dancer in red clothes and one dancer in blue clothes (these are the colors of the national flag of Berland). </li></ul><p>The agency has <span class="tex-span"><i>n</i></span> dancers, and their number can be less than <span class="tex-span">3<i>m</i></span>. That is, some dancers will probably have to dance in more than one dance. All of your dancers must dance on the party. However, if some dance has two or more dancers from a previous dance, then the current dance stops being spectacular. Your agency cannot allow that to happen, so each dance has at most one dancer who has danced in some previous dance. </p><p>You considered all the criteria and made the plan for the <span class="tex-span"><i>m</i></span> dances: each dance had three dancers participating in it. Your task is to determine the clothes color for each of the <span class="tex-span"><i>n</i></span> dancers so that the President's third condition fulfilled: each dance must have a dancer in white, a dancer in red and a dancer in blue. The dancers cannot change clothes between the dances.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of dancers and the number of dances, correspondingly. Then <span class="tex-span"><i>m</i></span> lines follow, describing the dances in the order of dancing them. The <span class="tex-span"><i>i</i></span>-th line contains three distinct integers — the numbers of the dancers that take part in the <span class="tex-span"><i>i</i></span>-th dance. The dancers are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Each dancer takes part in at least one dance.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th number must represent the color of the <span class="tex-span"><i>i</i></span>-th dancer's clothes (<span class="tex-span">1</span> for white, <span class="tex-span">2</span> for red, <span class="tex-span">3</span> for blue). If there are multiple valid solutions, print any of them. It is guaranteed that at least one solution exists.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of dancers and the number of dances, correspondingly. Then <span class="tex-span"><i>m</i></span> lines follow, describing the dances in the order of dancing them. The <span class="tex-span"><i>i</i></span>-th line contains three distinct integers — the numbers of the dancers that take part in the <span class="tex-span"><i>i</i></span>-th dance. The dancers are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Each dancer takes part in at least one dance.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th number must represent the color of the <span class="tex-span"><i>i</i></span>-th dancer's clothes (<span class="tex-span">1</span> for white, <span class="tex-span">2</span> for red, <span class="tex-span">3</span> for blue). If there are multiple valid solutions, print any of them. It is guaranteed that at least one solution exists.</p>





```input1
7 3
1 2 3
1 4 5
4 6 7

```




```input2
9 3
3 6 9
2 5 8
1 4 7

```




```input3
5 2
4 1 5
3 1 2

```




```output1
1 2 3 3 2 2 1 

```




```output2
1 1 1 2 2 2 3 3 3 

```




```output3
2 3 1 1 3 

```


