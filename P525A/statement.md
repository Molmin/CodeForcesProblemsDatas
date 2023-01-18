## Description

<div><p>After a hard day Vitaly got very hungry and he wants to eat his favorite potato pie. But it's not that simple. Vitaly is in the first room of the house with <span class="tex-span"><i>n</i></span> room located in a line and numbered starting from one from left to right. You can go from the first room to the second room, from the second room to the third room and so on — you can go from the (<span class="tex-span"><i>n</i> - 1</span>)-th room to the <span class="tex-span"><i>n</i></span>-th room. Thus, you can go to room <span class="tex-span"><i>x</i></span> only from room <span class="tex-span"><i>x</i> - 1</span>.</p><p>The potato pie is located in the <span class="tex-span"><i>n</i></span>-th room and Vitaly needs to go there. </p><p>Each pair of consecutive rooms has a door between them. In order to go to room <span class="tex-span"><i>x</i></span> from room <span class="tex-span"><i>x</i> - 1</span>, you need to open the door between the rooms with the corresponding key. </p><p>In total the house has several types of doors (represented by uppercase Latin letters) and several types of keys (represented by lowercase Latin letters). The key of type <span class="tex-span"><i>t</i></span> can open the door of type <span class="tex-span"><i>T</i></span> if and only if <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>T</i></span> are the same letter, written in different cases. For example, key <span class="tex-font-style-tt">f</span> can open door <span class="tex-font-style-tt">F</span>.</p><p>Each of the first <span class="tex-span"><i>n</i> - 1</span> rooms contains exactly one key of some type that Vitaly can use to get to next rooms. Once the door is open with some key, Vitaly won't get the key from the keyhole but he will immediately run into the next room. In other words, each key can open no more than one door.</p><p>Vitaly realizes that he may end up in some room without the key that opens the door to the next room. Before the start his run for the potato pie Vitaly can buy any number of keys of any type that is guaranteed to get to room <span class="tex-span"><i>n</i></span>.</p><p>Given the plan of the house, Vitaly wants to know what is the minimum number of keys he needs to buy to surely get to the room <span class="tex-span"><i>n</i></span>, which has a delicious potato pie. Write a program that will help Vitaly find out this number.</p></div><div class="input-specification"><p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;—&nbsp;the number of rooms in the house.</p><p>The second line of the input contains string <span class="tex-span"><i>s</i></span> of length <span class="tex-span">2·<i>n</i> - 2</span>. Let's number the elements of the string from left to right, starting from one. </p><p>The odd positions in the given string <span class="tex-span"><i>s</i></span> contain lowercase Latin letters&nbsp;—&nbsp;the types of the keys that lie in the corresponding rooms. Thus, each odd position <span class="tex-span"><i>i</i></span> of the given string <span class="tex-span"><i>s</i></span> contains a lowercase Latin letter — the type of the key that lies in room number <span class="tex-span">(<i>i</i> + 1) / 2</span>.</p><p>The even positions in the given string contain uppercase Latin letters — the types of doors between the rooms. Thus, each even position <span class="tex-span"><i>i</i></span> of the given string <span class="tex-span"><i>s</i></span> contains an uppercase letter — the type of the door that leads from room <span class="tex-span"><i>i</i> / 2</span> to room <span class="tex-span"><i>i</i> / 2 + 1</span>.</p></div><div class="output-specification"><p>Print the only integer — the minimum number of keys that Vitaly needs to buy to surely get from room one to room <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;—&nbsp;the number of rooms in the house.</p><p>The second line of the input contains string <span class="tex-span"><i>s</i></span> of length <span class="tex-span">2·<i>n</i> - 2</span>. Let's number the elements of the string from left to right, starting from one. </p><p>The odd positions in the given string <span class="tex-span"><i>s</i></span> contain lowercase Latin letters&nbsp;—&nbsp;the types of the keys that lie in the corresponding rooms. Thus, each odd position <span class="tex-span"><i>i</i></span> of the given string <span class="tex-span"><i>s</i></span> contains a lowercase Latin letter — the type of the key that lies in room number <span class="tex-span">(<i>i</i> + 1) / 2</span>.</p><p>The even positions in the given string contain uppercase Latin letters — the types of doors between the rooms. Thus, each even position <span class="tex-span"><i>i</i></span> of the given string <span class="tex-span"><i>s</i></span> contains an uppercase letter — the type of the door that leads from room <span class="tex-span"><i>i</i> / 2</span> to room <span class="tex-span"><i>i</i> / 2 + 1</span>.</p>

## Output

<p>Print the only integer — the minimum number of keys that Vitaly needs to buy to surely get from room one to room <span class="tex-span"><i>n</i></span>.</p>





```input1
3
aAbB

```




```input2
4
aBaCaB

```




```input3
5
xYyXzZaZ

```




```output1
0

```




```output2
3

```




```output3
2

```


