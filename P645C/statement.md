## Description

<div><p>In an attempt to escape the Mischievous Mess Makers' antics, Farmer John has abandoned his farm and is traveling to the other side of Bovinia. During the journey, he and his <span class="tex-span"><i>k</i></span> cows have decided to stay at the luxurious Grand Moo-dapest Hotel. The hotel consists of <span class="tex-span"><i>n</i></span> rooms located in a row, some of which are occupied.</p><p>Farmer John wants to book a set of <span class="tex-span"><i>k</i> + 1</span> currently unoccupied rooms for him and his cows. He wants his cows to stay as safe as possible, so he wishes to minimize the maximum distance from his room to the room of his cow. The distance between rooms <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> is defined as <span class="tex-span">|<i>j</i> - <i>i</i>|</span>. Help Farmer John protect his cows by calculating this minimum possible distance.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> &lt; <i>n</i> ≤ 100 000</span>)&nbsp;— the number of rooms in the hotel and the number of cows travelling with Farmer John.</p><p>The second line contains a string of length <span class="tex-span"><i>n</i></span> describing the rooms. The <span class="tex-span"><i>i</i></span>-th character of the string will be '<span class="tex-font-style-tt">0</span>' if the <span class="tex-span"><i>i</i></span>-th room is free, and '<span class="tex-font-style-tt">1</span>' if the <span class="tex-span"><i>i</i></span>-th room is occupied. It is guaranteed that at least <span class="tex-span"><i>k</i> + 1</span> characters of this string are '<span class="tex-font-style-tt">0</span>', so there exists at least one possible choice of <span class="tex-span"><i>k</i> + 1</span> rooms for Farmer John and his cows to stay in.</p></div><div class="output-specification"><p>Print the minimum possible distance between Farmer John's room and his farthest cow.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> &lt; <i>n</i> ≤ 100 000</span>)&nbsp;— the number of rooms in the hotel and the number of cows travelling with Farmer John.</p><p>The second line contains a string of length <span class="tex-span"><i>n</i></span> describing the rooms. The <span class="tex-span"><i>i</i></span>-th character of the string will be '<span class="tex-font-style-tt">0</span>' if the <span class="tex-span"><i>i</i></span>-th room is free, and '<span class="tex-font-style-tt">1</span>' if the <span class="tex-span"><i>i</i></span>-th room is occupied. It is guaranteed that at least <span class="tex-span"><i>k</i> + 1</span> characters of this string are '<span class="tex-font-style-tt">0</span>', so there exists at least one possible choice of <span class="tex-span"><i>k</i> + 1</span> rooms for Farmer John and his cows to stay in.</p>

## Output

<p>Print the minimum possible distance between Farmer John's room and his farthest cow.</p>





```input1
7 2
0100100

```




```input2
5 1
01010

```




```input3
3 2
000

```




```output1
2

```




```output2
2

```




```output3
1

```



## Note

<p>In the first sample, Farmer John can book room <span class="tex-span">3</span> for himself, and rooms <span class="tex-span">1</span> and <span class="tex-span">4</span> for his cows. The distance to the farthest cow is <span class="tex-span">2</span>. Note that it is impossible to make this distance <span class="tex-span">1</span>, as there is no block of three consecutive unoccupied rooms.</p><p>In the second sample, Farmer John can book room <span class="tex-span">1</span> for himself and room <span class="tex-span">3</span> for his single cow. The distance between him and his cow is <span class="tex-span">2</span>.</p><p>In the third sample, Farmer John books all three available rooms, taking the middle room for himself so that both cows are next to him. His distance from the farthest cow is <span class="tex-span">1</span>.</p>
