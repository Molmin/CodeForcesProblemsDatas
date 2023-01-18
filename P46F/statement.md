## Description

<div><p>Today you are to solve the problem even the famous Hercule Poirot can't cope with! That's why this crime has not yet been solved and this story was never included in Agatha Christie's detective story books. </p><p>You are not informed on what crime was committed, when and where the corpse was found and other details. We only know that the crime was committed in a house that has <span class="tex-span"><i>n</i></span> rooms and <span class="tex-span"><i>m</i></span> doors between the pairs of rooms. The house residents are very suspicious, that's why all the doors can be locked with keys and all the keys are different. According to the provided evidence on Thursday night all the doors in the house were locked, and it is known in what rooms were the residents, and what kind of keys had any one of them. The same is known for the Friday night, when all the doors were also locked. On Friday it was raining heavily, that's why nobody left the house and nobody entered it. During the day the house residents could</p><ul> <li> open and close doors to the neighboring rooms using the keys at their disposal (every door can be opened and closed from each side); </li><li> move freely from a room to a room if a corresponding door is open; </li><li> give keys to one another, being in one room. </li></ul> <p>"Little grey matter" of Hercule Poirot are not capable of coping with such amount of information. Find out if the positions of people and keys on the Thursday night could result in the positions on Friday night, otherwise somebody among the witnesses is surely lying.</p></div><div class="input-specification"><p>The first line contains three preset integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> и <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 1000</span>) — the number of rooms, the number of doors and the number of house residents respectively. The next <span class="tex-span"><i>m</i></span> lines contain pairs of room numbers which join the doors. The rooms are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. There cannot be more that one door between the pair of rooms. No door connects a room with itself. The next <span class="tex-span"><i>k</i></span> lines describe the residents' position on the first night. Every line contains a resident's name (a non-empty line consisting of no more than <span class="tex-span">10</span> Latin letters), then after a space follows the room number, then, after a space — the number of keys the resident has. Then follow written space-separated numbers of the doors that can be unlocked by these keys. The doors are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in the order in which they are described in the input data. All the residents have different names, uppercase and lowercase letters considered to be different. Every <span class="tex-span"><i>m</i></span> keys occurs exactly once in the description. Multiple people may be present in one room, some rooms may be empty. The next <span class="tex-span"><i>k</i></span> lines describe the position of the residents on the second night in the very same format. It is guaranteed that in the second night's description the residents' names remain the same and every <span class="tex-span"><i>m</i></span> keys occurs exactly once.</p></div><div class="output-specification"><p>Print "YES" (without quotes) if the second arrangement can result from the first one, otherwise, print "NO".</p></div>

## Input

<p>The first line contains three preset integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> и <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 1000</span>) — the number of rooms, the number of doors and the number of house residents respectively. The next <span class="tex-span"><i>m</i></span> lines contain pairs of room numbers which join the doors. The rooms are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. There cannot be more that one door between the pair of rooms. No door connects a room with itself. The next <span class="tex-span"><i>k</i></span> lines describe the residents' position on the first night. Every line contains a resident's name (a non-empty line consisting of no more than <span class="tex-span">10</span> Latin letters), then after a space follows the room number, then, after a space — the number of keys the resident has. Then follow written space-separated numbers of the doors that can be unlocked by these keys. The doors are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in the order in which they are described in the input data. All the residents have different names, uppercase and lowercase letters considered to be different. Every <span class="tex-span"><i>m</i></span> keys occurs exactly once in the description. Multiple people may be present in one room, some rooms may be empty. The next <span class="tex-span"><i>k</i></span> lines describe the position of the residents on the second night in the very same format. It is guaranteed that in the second night's description the residents' names remain the same and every <span class="tex-span"><i>m</i></span> keys occurs exactly once.</p>

## Output

<p>Print "YES" (without quotes) if the second arrangement can result from the first one, otherwise, print "NO".</p>





```input1
2 1 2
1 2
Dmitry 1 1 1
Natalia 2 0
Natalia 1 1 1
Dmitry 2 0

```




```input2
4 4 3
1 3
1 2
2 3
3 4
Artem 1 1 4
Dmitry 1 1 2
Edvard 4 2 1 3
Artem 2 0
Dmitry 1 0
Edvard 4 4 1 2 3 4

```




```output1
YES

```




```output2
NO

```


