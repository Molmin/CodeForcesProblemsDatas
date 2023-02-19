## Description

<div><p>It's that time of the year, Felicity is around the corner and you can see people celebrating all around the Himalayan region. The Himalayan region has <span class="tex-span"><i>n</i></span> gyms. The <span class="tex-span"><i>i</i></span>-th gym has <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> Pokemon in it. There are <span class="tex-span"><i>m</i></span> distinct Pokemon types in the Himalayan region numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. There is a special evolution camp set up in the fest which claims to evolve any Pokemon. The type of a Pokemon could change after evolving, subject to the constraint that if two Pokemon have the same type before evolving, they will have the same type after evolving. Also, if two Pokemon have different types before evolving, they will have different types after evolving. It is also possible that a Pokemon has the same type before and after evolving. </p><p>Formally, an <span class="tex-font-style-it">evolution plan</span> is a permutation <span class="tex-span"><i>f</i></span> of <span class="tex-span">{1, 2, ..., <i>m</i>}</span>, such that <span class="tex-span"><i>f</i>(<i>x</i>) = <i>y</i></span> means that a Pokemon of type <span class="tex-span"><i>x</i></span> evolves into a Pokemon of type <span class="tex-span"><i>y</i></span>.</p><p>The gym leaders are intrigued by the special evolution camp and all of them plan to evolve their Pokemons. The protocol of the mountain states that in each gym, for every type of Pokemon, the number of Pokemon of that type before evolving any Pokemon should be equal the number of Pokemon of that type after evolving all the Pokemons according to the evolution plan. They now want to find out how many distinct <span class="tex-font-style-it">evolution plans</span> exist which satisfy the protocol.</p><p>Two evolution plans <span class="tex-span"><i>f</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>f</i><sub class="lower-index">2</sub></span> are distinct, if they have at least one Pokemon type evolving into a different Pokemon type in the two plans, i. e. there exists an <span class="tex-span"><i>i</i></span> such that <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>(<i>i</i>) ≠ <i>f</i><sub class="lower-index">2</sub>(<i>i</i>)</span>.</p><p>Your task is to find how many distinct <span class="tex-font-style-it">evolution plans</span> are possible such that if all Pokemon in all the gyms are evolved, the number of Pokemon of each type in each of the gyms remains the same. As the answer can be large, output it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of gyms and the number of Pokemon types.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the description of Pokemons in the gyms. The <span class="tex-span"><i>i</i></span>-th of these lines begins with the integer <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of Pokemon in the <span class="tex-span"><i>i</i></span>-th gym. After that <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> integers follow, denoting types of the Pokemons in the <span class="tex-span"><i>i</i></span>-th gym. Each of these integers is between <span class="tex-span">1</span> and <span class="tex-span"><i>m</i></span>.</p><p>The total number of Pokemons (the sum of all <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span>) does not exceed <span class="tex-span">5·10<sup class="upper-index">5</sup></span>.</p></div><div class="output-specification"><p>Output the number of valid evolution plans modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the number of gyms and the number of Pokemon types.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the description of Pokemons in the gyms. The <span class="tex-span"><i>i</i></span>-th of these lines begins with the integer <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>g</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of Pokemon in the <span class="tex-span"><i>i</i></span>-th gym. After that <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span> integers follow, denoting types of the Pokemons in the <span class="tex-span"><i>i</i></span>-th gym. Each of these integers is between <span class="tex-span">1</span> and <span class="tex-span"><i>m</i></span>.</p><p>The total number of Pokemons (the sum of all <span class="tex-span"><i>g</i><sub class="lower-index"><i>i</i></sub></span>) does not exceed <span class="tex-span">5·10<sup class="upper-index">5</sup></span>.</p>

## Output

<p>Output the number of valid evolution plans modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2 3
2 1 2
2 2 3

```




```input2
1 3
3 1 2 3

```




```input3
2 4
2 1 2
3 2 3 4

```




```input4
2 2
3 2 2 1
2 1 2

```




```input5
3 7
2 1 2
2 3 4
3 5 6 7

```




```output1
1

```




```output2
6

```




```output3
2

```




```output4
1

```




```output5
24

```



## Note

<p>In the first case, the only possible evolution plan is: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://vVxzbegF.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>In the second case, any permutation of <span class="tex-span">(1,  2,  3)</span> is valid.</p><p>In the third case, there are two possible plans: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://4faQHVtp.png" style="max-width: 100.0%;max-height: 100.0%;"></center> <center class="tex-equation"><img align="middle" class="tex-formula" src="file://YDM2bYsY.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>In the fourth case, the only possible evolution plan is: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://QdQfzkvQ.png" style="max-width: 100.0%;max-height: 100.0%;"></center>
