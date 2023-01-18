## Description

<div><p>Anya has bought a new smartphone that uses <span class="tex-font-style-underline">Berdroid</span> operating system. The smartphone menu has exactly <span class="tex-span"><i>n</i></span> applications, each application has its own icon. The icons are located on different screens, one screen contains <span class="tex-span"><i>k</i></span> icons. The icons from the first to the <span class="tex-span"><i>k</i></span>-th one are located on the first screen, from the <span class="tex-span">(<i>k</i> + 1)</span>-th to the <span class="tex-span">2<i>k</i></span>-th ones are on the second screen and so on (the last screen may be partially empty).</p><p>Initially the smartphone menu is showing the screen number <span class="tex-span">1</span>. To launch the application with the icon located on the screen <span class="tex-span"><i>t</i></span>, Anya needs to make the following gestures: first she scrolls to the required screen number <span class="tex-span"><i>t</i></span>, by making <span class="tex-span"><i>t</i> - 1</span> gestures (if the icon is on the screen <span class="tex-span"><i>t</i></span>), and then make another gesture — press the icon of the required application exactly once to launch it.</p><p>After the application is launched, the menu returns to the first screen. That is, to launch the next application you need to scroll through the menu again starting from the screen number <span class="tex-span">1</span>.</p><p>All applications are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. We know a certain order in which the icons of the applications are located in the menu at the beginning, but it changes as long as you use the operating system. <span class="tex-font-style-underline">Berdroid</span> is intelligent system, so it changes the order of the icons by moving the more frequently used icons to the beginning of the list. Formally, right after an application is launched, Berdroid swaps the application icon and the icon of a preceding application (that is, the icon of an application on the position that is smaller by one in the order of menu). The preceding icon may possibly be located on the adjacent screen. The only exception is when the icon of the launched application already occupies the first place, in this case the icon arrangement doesn't change.</p><p>Anya has planned the order in which she will launch applications. How many gestures should Anya make to launch the applications in the planned order? </p><p>Note that one application may be launched multiple times.</p></div><div class="input-specification"><p>The first line of the input contains three numbers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;—&nbsp;the number of applications that Anya has on her smartphone, the number of applications that will be launched and the number of icons that are located on the same screen.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers, permutation <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>&nbsp;—&nbsp;the initial order of icons from left to right in the menu (from the first to the last one), <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;—&nbsp; is the id of the application, whose icon goes <span class="tex-span"><i>i</i></span>-th in the menu. Each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> occurs exactly once among <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub>(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>&nbsp;—&nbsp;the ids of the launched applications in the planned order. One application may be launched multiple times.</p></div><div class="output-specification"><p>Print a single number — the number of gestures that Anya needs to make to launch all the applications in the desired order.</p></div>

## Input

<p>The first line of the input contains three numbers <span class="tex-span"><i>n</i>, <i>m</i>, <i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i>, <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;—&nbsp;the number of applications that Anya has on her smartphone, the number of applications that will be launched and the number of icons that are located on the same screen.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers, permutation <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>&nbsp;—&nbsp;the initial order of icons from left to right in the menu (from the first to the last one), <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;—&nbsp; is the id of the application, whose icon goes <span class="tex-span"><i>i</i></span>-th in the menu. Each integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> occurs exactly once among <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The third line contains <span class="tex-span"><i>m</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub>(1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span>&nbsp;—&nbsp;the ids of the launched applications in the planned order. One application may be launched multiple times.</p>

## Output

<p>Print a single number — the number of gestures that Anya needs to make to launch all the applications in the desired order.</p>





```input1
8 3 3
1 2 3 4 5 6 7 8
7 8 1

```




```input2
5 4 2
3 1 5 2 4
4 4 4 4

```




```output1
7

```




```output2
8

```



## Note

<p>In the first test the initial configuration looks like <span class="tex-span">(123)(456)(78)</span>, that is, the first screen contains icons of applications <span class="tex-span">1, 2, 3</span>, the second screen contains icons <span class="tex-span">4, 5, 6</span>, the third screen contains icons <span class="tex-span">7, 8</span>. </p><p>After application <span class="tex-span">7</span> is launched, we get the new arrangement of the icons&nbsp;—&nbsp;<span class="tex-span">(123)(457)(68)</span>. To launch it Anya makes <span class="tex-span">3</span> gestures. </p><p>After application <span class="tex-span">8</span> is launched, we get configuration <span class="tex-span">(123)(457)(86)</span>. To launch it Anya makes <span class="tex-span">3</span> gestures. </p><p>After application <span class="tex-span">1</span> is launched, the arrangement of icons in the menu doesn't change. To launch it Anya makes <span class="tex-span">1</span> gesture.</p><p>In total, Anya makes <span class="tex-span">7</span> gestures.</p>
