## Description

<div><p>Limak is a little polar bear. He loves connecting with other bears via social networks. He has <span class="tex-span"><i>n</i></span> friends and his relation with the <span class="tex-span"><i>i</i></span>-th of them is described by a unique integer <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. The bigger this value is, the better the friendship is. No two friends have the same value <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Spring is starting and the Winter sleep is over for bears. Limak has just woken up and logged in. All his friends still sleep and thus none of them is online. Some (maybe all) of them will appear online in the next hours, one at a time.</p><p>The system displays friends who are online. On the screen there is space to display at most <span class="tex-span"><i>k</i></span> friends. If there are more than <span class="tex-span"><i>k</i></span> friends online then the system displays only <span class="tex-span"><i>k</i></span> best of them&nbsp;— those with biggest <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Your task is to handle queries of two types:</p><ul> <li> "<span class="tex-font-style-tt">1 id</span>"&nbsp;— Friend <span class="tex-span"><i>id</i></span> becomes online. It's guaranteed that he wasn't online before. </li><li> "<span class="tex-font-style-tt">2 id</span>"&nbsp;— Check whether friend <span class="tex-span"><i>id</i></span> is displayed by the system. Print "<span class="tex-font-style-tt">YES</span>" or "<span class="tex-font-style-tt">NO</span>" in a separate line. </li></ul><p>Are you able to help Limak and answer all queries of the second type?</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 150 000, 1 ≤ <i>k</i> ≤ <i>min</i>(6, <i>n</i>)</span>)&nbsp;— the number of friends, the maximum number of displayed online friends and the number of queries, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> describes how good is Limak's relation with the <span class="tex-span"><i>i</i></span>-th friend.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 2, 1 ≤ <i>id</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the <span class="tex-span"><i>i</i></span>-th query. If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 1</span> then a friend <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> becomes online. If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 2</span> then you should check whether a friend <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> is displayed.</p><p>It's guaranteed that no two queries of the first type will have the same <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> becuase one friend can't become online twice. Also, it's guaranteed that at least one query will be of the second type (<span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 2</span>) so the output won't be empty.</p></div><div class="output-specification"><p>For each query of the second type print one line with the answer&nbsp;— "<span class="tex-font-style-tt">YES</span>" (without quotes) if the given friend is displayed and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 150 000, 1 ≤ <i>k</i> ≤ <i>min</i>(6, <i>n</i>)</span>)&nbsp;— the number of friends, the maximum number of displayed online friends and the number of queries, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> describes how good is Limak's relation with the <span class="tex-span"><i>i</i></span>-th friend.</p><p>The <span class="tex-span"><i>i</i></span>-th of the following <span class="tex-span"><i>q</i></span> lines contains two integers <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 2, 1 ≤ <i>id</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>)&nbsp;— the <span class="tex-span"><i>i</i></span>-th query. If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 1</span> then a friend <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> becomes online. If <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 2</span> then you should check whether a friend <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> is displayed.</p><p>It's guaranteed that no two queries of the first type will have the same <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub></span> becuase one friend can't become online twice. Also, it's guaranteed that at least one query will be of the second type (<span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub> = 2</span>) so the output won't be empty.</p>

## Output

<p>For each query of the second type print one line with the answer&nbsp;— "<span class="tex-font-style-tt">YES</span>" (without quotes) if the given friend is displayed and "<span class="tex-font-style-tt">NO</span>" (without quotes) otherwise.</p>





```input1
4 2 8
300 950 500 200
1 3
2 4
2 3
1 1
1 2
2 1
2 2
2 3

```




```input2
6 3 9
50 20 51 17 99 24
1 3
1 4
1 5
1 2
2 4
2 2
1 1
2 4
2 3

```




```output1
NO
YES
NO
YES
YES

```




```output2
NO
YES
NO
YES

```



## Note

<p>In the first sample, Limak has <span class="tex-span">4</span> friends who all sleep initially. At first, the system displays nobody because nobody is online. There are the following <span class="tex-span">8</span> queries:</p><ol> <li> "<span class="tex-font-style-tt">1 3</span>"&nbsp;— Friend <span class="tex-span">3</span> becomes online. </li><li> "<span class="tex-font-style-tt">2 4</span>"&nbsp;— We should check if friend <span class="tex-span">4</span> is displayed. He isn't even online and thus we print "<span class="tex-font-style-tt">NO</span>". </li><li> "<span class="tex-font-style-tt">2 3</span>"&nbsp;— We should check if friend <span class="tex-span">3</span> is displayed. Right now he is the only friend online and the system displays him. We should print "<span class="tex-font-style-tt">YES</span>". </li><li> "<span class="tex-font-style-tt">1 1</span>"&nbsp;— Friend <span class="tex-span">1</span> becomes online. The system now displays both friend <span class="tex-span">1</span> and friend <span class="tex-span">3</span>. </li><li> "<span class="tex-font-style-tt">1 2</span>"&nbsp;— Friend <span class="tex-span">2</span> becomes online. There are <span class="tex-span">3</span> friends online now but we were given <span class="tex-span"><i>k</i> = 2</span> so only two friends can be displayed. Limak has worse relation with friend <span class="tex-span">1</span> than with other two online friends (<span class="tex-span"><i>t</i><sub class="lower-index">1</sub> &lt; <i>t</i><sub class="lower-index">2</sub>, <i>t</i><sub class="lower-index">3</sub></span>) so friend <span class="tex-span">1</span> won't be displayed </li><li> "<span class="tex-font-style-tt">2 1</span>"&nbsp;— Print "<span class="tex-font-style-tt">NO</span>". </li><li> "<span class="tex-font-style-tt">2 2</span>"&nbsp;— Print "<span class="tex-font-style-tt">YES</span>". </li><li> "<span class="tex-font-style-tt">2 3</span>"&nbsp;— Print "<span class="tex-font-style-tt">YES</span>". </li></ol>
