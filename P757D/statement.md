## Description

<div><p>The gym leaders were fascinated by the evolutions which took place at Felicity camp. So, they were curious to know about the secret behind evolving Pokemon. </p><p>The organizers of the camp gave the gym leaders a PokeBlock, a sequence of <span class="tex-span"><i>n</i></span> ingredients. Each ingredient can be of type <span class="tex-span">0</span> or <span class="tex-span">1</span>. Now the organizers told the gym leaders that to evolve a Pokemon of type <span class="tex-span"><i>k</i></span> (<span class="tex-span"><i>k</i> ≥ 2</span>), they need to make a valid set of <span class="tex-span"><i>k</i></span> cuts on the PokeBlock to get smaller blocks.</p><p>Suppose the given PokeBlock sequence is <span class="tex-span"><i>b</i><sub class="lower-index">0</sub><i>b</i><sub class="lower-index">1</sub><i>b</i><sub class="lower-index">2</sub>... <i>b</i><sub class="lower-index"><i>n</i> - 1</sub></span>. You have a choice of making cuts at <span class="tex-span"><i>n</i> + 1</span> places, i.e., Before <span class="tex-span"><i>b</i><sub class="lower-index">0</sub></span>, between <span class="tex-span"><i>b</i><sub class="lower-index">0</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span>, between <span class="tex-span"><i>b</i><sub class="lower-index">1</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index">2</sub></span>, ..., between <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i> - 2</sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i> - 1</sub></span>, and after <span class="tex-span"><i>b</i><sub class="lower-index"><i>n</i> - 1</sub></span>.</p><p>The <span class="tex-span"><i>n</i> + 1</span> choices of making cuts are as follows (where a <span class="tex-font-style-tt">|</span> denotes a possible cut):</p><center class="tex-equation"><span class="tex-span">| <i>b</i><sub class="lower-index">0</sub> | <i>b</i><sub class="lower-index">1</sub> | <i>b</i><sub class="lower-index">2</sub> | ... | <i>b</i><sub class="lower-index"><i>n</i> - 2</sub> | <i>b</i><sub class="lower-index"><i>n</i> - 1</sub> |</span></center><p>Consider a sequence of <span class="tex-span"><i>k</i></span> cuts. Now each pair of consecutive cuts will contain a binary string between them, formed from the ingredient types. The ingredients before the first cut and after the last cut are wasted, which is to say they are not considered. So there will be exactly <span class="tex-span"><i>k</i> - 1</span> such binary substrings. Every substring can be read as a binary number. Let <span class="tex-span"><i>m</i></span> be the maximum number out of the obtained numbers. If all the obtained numbers are positive and the set of the obtained numbers contains all integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>, then this set of cuts is said to be a valid set of cuts.</p><p>For example, suppose the given PokeBlock sequence is <span class="tex-span">101101001110</span> and we made <span class="tex-span">5</span> cuts in the following way:</p><center class="tex-equation"><span class="tex-span">10 | 11 | 010 | 01 | 1 | 10</span></center><p>So the <span class="tex-span">4</span> binary substrings obtained are: <span class="tex-span">11</span>, <span class="tex-span">010</span>, <span class="tex-span">01</span> and <span class="tex-span">1</span>, which correspond to the numbers <span class="tex-span">3</span>, <span class="tex-span">2</span>, <span class="tex-span">1</span> and <span class="tex-span">1</span> respectively. Here <span class="tex-span"><i>m</i> = 3</span>, as it is the maximum value among the obtained numbers. And all the obtained numbers are positive and we have obtained all integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Hence this set of cuts is a valid set of <span class="tex-span">5</span> cuts.</p><p>A Pokemon of type <span class="tex-span"><i>k</i></span> will evolve only if the PokeBlock is cut using a valid set of <span class="tex-span"><i>k</i></span> cuts. There can be many valid sets of the same size. Two valid sets of <span class="tex-span"><i>k</i></span> cuts are considered different if there is a cut in one set which is not there in the other set.</p><p>Let <span class="tex-span"><i>f</i>(<i>k</i>)</span> denote the number of valid sets of <span class="tex-span"><i>k</i></span> cuts. Find the value of <img align="middle" class="tex-formula" src="file://N7n334y1.png" style="max-width: 100.0%;max-height: 100.0%;">. Since the value of <span class="tex-span"><i>s</i></span> can be very large, output <span class="tex-span"><i>s</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The input consists of two lines. The first line consists an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 75</span>)&nbsp;— the length of the PokeBlock. The next line contains the PokeBlock, a binary string of length <span class="tex-span"><i>n</i></span>.</p></div><div class="output-specification"><p>Output a single integer, containing the answer to the problem, i.e., the value of <span class="tex-span"><i>s</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The input consists of two lines. The first line consists an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 75</span>)&nbsp;— the length of the PokeBlock. The next line contains the PokeBlock, a binary string of length <span class="tex-span"><i>n</i></span>.</p>

## Output

<p>Output a single integer, containing the answer to the problem, i.e., the value of <span class="tex-span"><i>s</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
4
1011

```




```input2
2
10

```




```output1
10

```




```output2
1

```



## Note

<p>In the first sample, the sets of valid cuts are:</p><p>Size <span class="tex-span">2</span>: <span class="tex-font-style-tt">|1|011</span>, <span class="tex-font-style-tt">1|01|1</span>, <span class="tex-font-style-tt">10|1|1</span>, <span class="tex-font-style-tt">101|1|</span>.</p><p>Size <span class="tex-span">3</span>: <span class="tex-font-style-tt">|1|01|1</span>, <span class="tex-font-style-tt">|10|1|1</span>, <span class="tex-font-style-tt">10|1|1|</span>, <span class="tex-font-style-tt">1|01|1|</span>.</p><p>Size <span class="tex-span">4</span>: <span class="tex-font-style-tt">|10|1|1|</span>, <span class="tex-font-style-tt">|1|01|1|</span>.</p><p>Hence, <span class="tex-span"><i>f</i>(2) = 4</span>, <span class="tex-span"><i>f</i>(3) = 4</span> and <span class="tex-span"><i>f</i>(4) = 2</span>. So, the value of <span class="tex-span"><i>s</i> = 10</span>.</p><p>In the second sample, the set of valid cuts is:</p><p>Size <span class="tex-span">2</span>: |1|0.</p><p>Hence, <span class="tex-span"><i>f</i>(2) = 1</span> and <span class="tex-span"><i>f</i>(3) = 0</span>. So, the value of <span class="tex-span"><i>s</i> = 1</span>.</p>
