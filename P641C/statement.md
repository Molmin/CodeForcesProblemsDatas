## Description

<div><p>Little Artem is fond of dancing. Most of all dances Artem likes rueda&nbsp;— Cuban dance that is danced by pairs of boys and girls forming a circle and dancing together.</p><p>More detailed, there are <span class="tex-span"><i>n</i></span> pairs of boys and girls standing in a circle. Initially, boy number <span class="tex-span">1</span> dances with a girl number <span class="tex-span">1</span>, boy number <span class="tex-span">2</span> dances with a girl number <span class="tex-span">2</span> and so on. Girls are numbered in the clockwise order. During the dance different moves are announced and all pairs perform this moves. While performing moves boys move along the circle, while girls always stay at their initial position. For the purpose of this problem we consider two different types of moves:</p><ol> <li> Value <span class="tex-span"><i>x</i></span> and some direction are announced, and all boys move <span class="tex-span"><i>x</i></span> positions in the corresponding direction. </li><li> Boys dancing with even-indexed girls swap positions with boys who are dancing with odd-indexed girls. That is the one who was dancing with the girl <span class="tex-span">1</span> swaps with the one who was dancing with the girl number <span class="tex-span">2</span>, while the one who was dancing with girl number <span class="tex-span">3</span> swaps with the one who was dancing with the girl number <span class="tex-span">4</span> and so one. It's guaranteed that <span class="tex-span"><i>n</i></span> is even. </li></ol><p>Your task is to determine the final position of each boy.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1 000 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 2 000 000</span>)&nbsp;— the number of couples in the rueda and the number of commands to perform, respectively. It's guaranteed that <span class="tex-span"><i>n</i></span> is even.</p><p>Next <span class="tex-span"><i>q</i></span> lines contain the descriptions of the commands. Each command has type as the integer <span class="tex-span">1</span> or <span class="tex-span">2</span> first. Command of the first type is given as <span class="tex-span"><i>x</i></span> (<span class="tex-span"> - <i>n</i> ≤ <i>x</i> ≤ <i>n</i></span>), where <span class="tex-span">0 ≤ <i>x</i> ≤ <i>n</i></span> means all boys moves <span class="tex-span"><i>x</i></span> girls in clockwise direction, while <span class="tex-span"> - <i>x</i></span> means all boys move <span class="tex-span"><i>x</i></span> positions in counter-clockwise direction. There is no other input for commands of the second type.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them should be equal to the index of boy the <span class="tex-span"><i>i</i></span>-th girl is dancing with after performing all <span class="tex-span"><i>q</i></span> moves.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1 000 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 2 000 000</span>)&nbsp;— the number of couples in the rueda and the number of commands to perform, respectively. It's guaranteed that <span class="tex-span"><i>n</i></span> is even.</p><p>Next <span class="tex-span"><i>q</i></span> lines contain the descriptions of the commands. Each command has type as the integer <span class="tex-span">1</span> or <span class="tex-span">2</span> first. Command of the first type is given as <span class="tex-span"><i>x</i></span> (<span class="tex-span"> - <i>n</i> ≤ <i>x</i> ≤ <i>n</i></span>), where <span class="tex-span">0 ≤ <i>x</i> ≤ <i>n</i></span> means all boys moves <span class="tex-span"><i>x</i></span> girls in clockwise direction, while <span class="tex-span"> - <i>x</i></span> means all boys move <span class="tex-span"><i>x</i></span> positions in counter-clockwise direction. There is no other input for commands of the second type.</p>

## Output

<p>Output <span class="tex-span"><i>n</i></span> integers, the <span class="tex-span"><i>i</i></span>-th of them should be equal to the index of boy the <span class="tex-span"><i>i</i></span>-th girl is dancing with after performing all <span class="tex-span"><i>q</i></span> moves.</p>





```input1
6 3
1 2
2
1 2

```




```input2
2 3
1 1
2
1 -2

```




```input3
4 2
2
1 3

```




```output1
4 3 6 5 2 1

```




```output2
1 2

```




```output3
1 4 3 2

```


