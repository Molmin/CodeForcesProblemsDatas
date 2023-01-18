## Description

<div><p>During the break the schoolchildren, boys and girls, formed a queue of <span class="tex-span"><i>n</i></span> people in the canteen. Initially the children stood in the order they entered the canteen. However, after a while the boys started feeling awkward for standing in front of the girls in the queue and they started letting the girls move forward each second. </p><p>Let's describe the process more precisely. Let's say that the positions in the queue are sequentially numbered by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, at that the person in the position number <span class="tex-span">1</span> is served first. Then, if at time <span class="tex-span"><i>x</i></span> a boy stands on the <span class="tex-span"><i>i</i></span>-th position and a girl stands on the <span class="tex-span">(<i>i</i> + 1)</span>-th position, then at time <span class="tex-span"><i>x</i> + 1</span> the <span class="tex-span"><i>i</i></span>-th position will have a girl and the <span class="tex-span">(<i>i</i> + 1)</span>-th position will have a boy. The time is given in seconds.</p><p>You've got the initial position of the children, at the initial moment of time. Determine the way the queue is going to look after <span class="tex-span"><i>t</i></span> seconds.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>t</i> ≤ 50)</span>, which represent the number of children in the queue and the time after which the queue will transform into the arrangement you need to find. </p><p>The next line contains string <span class="tex-span"><i>s</i></span>, which represents the schoolchildren's initial arrangement. If the <span class="tex-span"><i>i</i></span>-th position in the queue contains a boy, then the <span class="tex-span"><i>i</i></span>-th character of string <span class="tex-span"><i>s</i></span> equals "<span class="tex-font-style-tt">B</span>", otherwise the <span class="tex-span"><i>i</i></span>-th character equals "<span class="tex-font-style-tt">G</span>".</p></div><div class="output-specification"><p>Print string <span class="tex-span"><i>a</i></span>, which describes the arrangement after <span class="tex-span"><i>t</i></span> seconds. If the <span class="tex-span"><i>i</i></span>-th position has a boy after the needed time, then the <span class="tex-span"><i>i</i></span>-th character <span class="tex-span"><i>a</i></span> must equal "<span class="tex-font-style-tt">B</span>", otherwise it must equal "<span class="tex-font-style-tt">G</span>".</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>t</i> ≤ 50)</span>, which represent the number of children in the queue and the time after which the queue will transform into the arrangement you need to find. </p><p>The next line contains string <span class="tex-span"><i>s</i></span>, which represents the schoolchildren's initial arrangement. If the <span class="tex-span"><i>i</i></span>-th position in the queue contains a boy, then the <span class="tex-span"><i>i</i></span>-th character of string <span class="tex-span"><i>s</i></span> equals "<span class="tex-font-style-tt">B</span>", otherwise the <span class="tex-span"><i>i</i></span>-th character equals "<span class="tex-font-style-tt">G</span>".</p>

## Output

<p>Print string <span class="tex-span"><i>a</i></span>, which describes the arrangement after <span class="tex-span"><i>t</i></span> seconds. If the <span class="tex-span"><i>i</i></span>-th position has a boy after the needed time, then the <span class="tex-span"><i>i</i></span>-th character <span class="tex-span"><i>a</i></span> must equal "<span class="tex-font-style-tt">B</span>", otherwise it must equal "<span class="tex-font-style-tt">G</span>".</p>





```input1
5 1
BGGBG

```




```input2
5 2
BGGBG

```




```input3
4 1
GGGB

```




```output1
GBGGB

```




```output2
GGBGB

```




```output3
GGGB

```


