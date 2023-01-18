## Description

<div><p>There is unrest in the Galactic Senate. Several thousand solar systems have declared their intentions to leave the Republic. Master Heidi needs to select the Jedi Knights who will go on peacekeeping missions throughout the galaxy. It is well-known that the success of any peacekeeping mission depends on the colors of the lightsabers of the Jedi who will go on that mission. </p><p>Heidi has <span class="tex-span"><i>n</i></span> Jedi Knights standing in front of her, each one with a lightsaber of one of <span class="tex-span"><i>m</i></span> possible colors. She knows that for the mission to be the most effective, she needs to select some contiguous interval of knights such that there are exactly <span class="tex-span"><i>k</i><sub class="lower-index">1</sub></span> knights with lightsabers of the first color, <span class="tex-span"><i>k</i><sub class="lower-index">2</sub></span> knights with lightsabers of the second color, <span class="tex-span">...</span>, <span class="tex-span"><i>k</i><sub class="lower-index"><i>m</i></sub></span> knights with lightsabers of the <span class="tex-span"><i>m</i></span>-th color.</p><p>However, since the last time, she has learned that it is not always possible to select such an interval. Therefore, she decided to ask some Jedi Knights to go on an indefinite unpaid vacation leave near certain pits on Tatooine, if you know what I mean. Help Heidi decide what is the minimum number of Jedi Knights that need to be let go before she is able to select the desired interval from the subsequence of remaining knights.</p></div><div class="input-specification"><p>The first line of the input contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>). The second line contains <span class="tex-span"><i>n</i></span> integers in the range <span class="tex-span">{1, 2, ..., <i>m</i>}</span> representing colors of the lightsabers of the subsequent Jedi Knights. The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>m</i></sub></span> (with <img align="middle" class="tex-formula" src="file://0PitDQzv.png" style="max-width: 100.0%;max-height: 100.0%;">) – the desired counts of Jedi Knights with lightsabers of each color from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p></div><div class="output-specification"><p>Output one number: the minimum number of Jedi Knights that need to be removed from the sequence so that, in what remains, there is an interval with the prescribed counts of lightsaber colors. If this is not possible, output <span class="tex-span"> - 1</span>.</p></div>

## Input

<p>The first line of the input contains <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ <i>n</i></span>). The second line contains <span class="tex-span"><i>n</i></span> integers in the range <span class="tex-span">{1, 2, ..., <i>m</i>}</span> representing colors of the lightsabers of the subsequent Jedi Knights. The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>k</i><sub class="lower-index">1</sub>, <i>k</i><sub class="lower-index">2</sub>, ..., <i>k</i><sub class="lower-index"><i>m</i></sub></span> (with <img align="middle" class="tex-formula" src="file://0PitDQzv.png" style="max-width: 100.0%;max-height: 100.0%;">) – the desired counts of Jedi Knights with lightsabers of each color from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p>

## Output

<p>Output one number: the minimum number of Jedi Knights that need to be removed from the sequence so that, in what remains, there is an interval with the prescribed counts of lightsaber colors. If this is not possible, output <span class="tex-span"> - 1</span>.</p>





```input1
8 3
3 3 1 2 2 1 1 3
3 1 1

```




```output1
1

```


