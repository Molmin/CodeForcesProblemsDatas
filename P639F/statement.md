## Description

<div><p>Limak is a smart brown bear who loves chemistry, reactions and transforming elements.</p><p>In Bearland (Limak's home) there are <span class="tex-span"><i>n</i></span> elements, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. There are also special machines, that can transform elements. Each machine is described by two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span> representing two elements, not necessarily distinct. One can use a machine either to transform an element <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> or to transform <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. Machines in Bearland aren't very resistant and each of them can be used <span class="tex-font-style-bf">at most once</span>. It is possible that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i></sub></span> and that many machines have the same pair <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Radewoosh is Limak's biggest enemy and rival. He wants to test Limak in the chemistry. They will meet tomorrow and both of them will bring all their machines. Limak has <span class="tex-span"><i>m</i></span> machines but he doesn't know much about his enemy. They agreed Radewoosh will choose two distinct elements, let's denote them as <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span>. Limak will be allowed to use both his and Radewoosh's machines. He may use zero or more (maybe even all) machines to achieve the goal, each machine at most once. Limak will start from an element <span class="tex-span"><i>x</i></span> and his task will be to first get an element <span class="tex-span"><i>y</i></span> and then to again get an element <span class="tex-span"><i>x</i></span>&nbsp;— <span class="tex-font-style-bf">then we say that he succeeds</span>. After that Radewoosh would agree that Limak knows the chemistry (and Radewoosh would go away).</p><p>Radewoosh likes some particular non-empty set of favorite elements and he will choose <span class="tex-span"><i>x</i>, <i>y</i></span> from that set. Limak doesn't know exactly which elements are in the set and also he doesn't know what machines Radewoosh has. Limak has heard <span class="tex-span"><i>q</i></span> gossips (queries) though and each of them consists of Radewoosh's machines and favorite elements. For each gossip Limak wonders if he would be able to <span class="tex-font-style-bf">succeed</span> tomorrow for every pair <span class="tex-span"><i>x</i>, <i>y</i></span> chosen from the set of favorite elements. If yes then print "<span class="tex-font-style-tt">YES</span>" (without the quotes). But if there exists a pair <span class="tex-span">(<i>x</i>, <i>y</i>)</span> from the given set that Limak wouldn't be able to succeed then you should print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 300 000, 0 ≤ <i>m</i> ≤ 300 000</span>)&nbsp;— the number of elements, the number of Limak's machines and the number of gossips, respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) describing one of Limak's machines.</p><p>Then, the description of <span class="tex-span"><i>q</i></span> gossips follows.</p><p>The first line of the description of the <span class="tex-span"><i>i</i></span>-th gossip contains two integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 300 000, 0 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 300 000</span>). The second line contains <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>x</i><sub class="lower-index"><i>i</i>, <i>n</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>n</i></span>)&nbsp;— Radewoosh's favorite elements in the <span class="tex-span"><i>i</i></span>-th gossip. Note that <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub> = 1</span> is allowed, in this case there are no pairs of distinct elements, so Limak automatically wins (the answer is "<span class="tex-font-style-tt">YES</span>"). Then <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> lines follow, each containing two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub>, <i>b</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub>, <i>b</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>) describing one of Radewoosh's machines in the <span class="tex-span"><i>i</i></span>-th gossip.</p><p>The sum of <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> over all gossips won't exceed <span class="tex-span">300 000</span>. Also, the sum of <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> over all gossips won't exceed <span class="tex-span">300 000</span>.</p><p><span class="tex-font-style-bf">Important:</span> Because we want you to process the gossips online, in order to know the elements in Radewoosh's favorite set and elements that his machines can transform, for on each number that denotes them in the input you should use following function:</p><pre class="verbatim">int rotate(int element)<br>{<br>   element=(element+R)%n;<br><br>   if (element==0) {<br>       element=n;<br>   }<br><br>   return element;<br>}<br></pre><p>where <span class="tex-span"><i>R</i></span> is initially equal to <span class="tex-span">0</span> and is increased by the number of the query any time the answer is "<span class="tex-font-style-tt">YES</span>". Queries are numbered starting with <span class="tex-span">1</span> in the order they appear in the input.</p></div><div class="output-specification"><p>You should print <span class="tex-span"><i>q</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain "<span class="tex-font-style-tt">YES</span>" (without quotes) if for the <span class="tex-span"><i>i</i></span>-th gossip <span class="tex-font-style-bf">for each pair</span> of elements <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (in the set <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>x</i><sub class="lower-index"><i>i</i>, <i>n</i><sub class="lower-index"><i>i</i></sub></sub></span>) Limak is able to succeed. Otherwise you should print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>q</i> ≤ 300 000, 0 ≤ <i>m</i> ≤ 300 000</span>)&nbsp;— the number of elements, the number of Limak's machines and the number of gossips, respectively.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) describing one of Limak's machines.</p><p>Then, the description of <span class="tex-span"><i>q</i></span> gossips follows.</p><p>The first line of the description of the <span class="tex-span"><i>i</i></span>-th gossip contains two integers <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>n</i><sub class="lower-index"><i>i</i></sub> ≤ 300 000, 0 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 300 000</span>). The second line contains <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-font-style-bf">distinct</span> integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>x</i><sub class="lower-index"><i>i</i>, <i>n</i><sub class="lower-index"><i>i</i></sub></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i>, <i>j</i></sub> ≤ <i>n</i></span>)&nbsp;— Radewoosh's favorite elements in the <span class="tex-span"><i>i</i></span>-th gossip. Note that <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub> = 1</span> is allowed, in this case there are no pairs of distinct elements, so Limak automatically wins (the answer is "<span class="tex-font-style-tt">YES</span>"). Then <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> lines follow, each containing two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub>, <i>b</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub>, <i>b</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>) describing one of Radewoosh's machines in the <span class="tex-span"><i>i</i></span>-th gossip.</p><p>The sum of <span class="tex-span"><i>n</i><sub class="lower-index"><i>i</i></sub></span> over all gossips won't exceed <span class="tex-span">300 000</span>. Also, the sum of <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> over all gossips won't exceed <span class="tex-span">300 000</span>.</p><p><span class="tex-font-style-bf">Important:</span> Because we want you to process the gossips online, in order to know the elements in Radewoosh's favorite set and elements that his machines can transform, for on each number that denotes them in the input you should use following function:</p><pre class="verbatim">int rotate(int element)<br>{<br>   element=(element+R)%n;<br><br>   if (element==0) {<br>       element=n;<br>   }<br><br>   return element;<br>}<br></pre><p>where <span class="tex-span"><i>R</i></span> is initially equal to <span class="tex-span">0</span> and is increased by the number of the query any time the answer is "<span class="tex-font-style-tt">YES</span>". Queries are numbered starting with <span class="tex-span">1</span> in the order they appear in the input.</p>

## Output

<p>You should print <span class="tex-span"><i>q</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain "<span class="tex-font-style-tt">YES</span>" (without quotes) if for the <span class="tex-span"><i>i</i></span>-th gossip <span class="tex-font-style-bf">for each pair</span> of elements <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> (in the set <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>x</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>x</i><sub class="lower-index"><i>i</i>, <i>n</i><sub class="lower-index"><i>i</i></sub></sub></span>) Limak is able to succeed. Otherwise you should print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
6 5 4
1 2
2 3
3 4
2 4
5 6
2 0
4 2
2 1
6 2
3 4
3 2
6 3 4
2 5
4 6
2 1
1 2
1 2

```




```input2
7 6 2
1 2
1 3
2 4
2 5
3 6
3 7
7 2
1 2 3 4 5 6 7
4 5
6 7
7 2
1 2 3 4 5 6 7
4 6
5 7

```




```output1
YES
NO
YES
YES

```




```output2
NO
YES

```



## Note

<p>Lets look at first sample:</p><p>In first gossip Radewoosh's favorite set is <span class="tex-span">{4, 2}</span> and he has no machines. Limak can tranform element <span class="tex-span">4</span> into <span class="tex-span">2</span> (so half of a task is complete) and then <span class="tex-span">2</span> into <span class="tex-span">3</span>, and <span class="tex-span">3</span> into <span class="tex-span">4</span>. Answer is "<span class="tex-font-style-tt">YES</span>", so <span class="tex-span"><i>R</i></span> is increased by <span class="tex-span">1</span>.</p><p>In second gossip set in the input is denoted by <span class="tex-span">{6, 2}</span> and machine by <span class="tex-span">(3, 4)</span>, but <span class="tex-span"><i>R</i></span> is equal to <span class="tex-span">1</span>, so set is <span class="tex-span">{1, 3}</span> and machine is <span class="tex-span">(4, 5)</span>. Answer is "<span class="tex-font-style-tt">NO</span>", so <span class="tex-span"><i>R</i></span> isn't changed.</p><p>In third gossip set <span class="tex-span">{6, 4, 3}</span> and machines <span class="tex-span">(2, 5)</span> and <span class="tex-span">(4, 6)</span> are deciphered to be <span class="tex-span">{1, 5, 4}</span>, <span class="tex-span">(3, 6)</span> and <span class="tex-span">(5, 1)</span>.</p><p>Consider Radewoosh's choices: </p><ul> <li> If he chooses elements <span class="tex-span">1</span> and <span class="tex-span">5</span>, then Limak is able to transform <span class="tex-span">1</span> into <span class="tex-span">5</span>, then <span class="tex-span">6</span> into <span class="tex-span">3</span>, <span class="tex-span">3</span> into <span class="tex-span">2</span> and <span class="tex-span">2</span> into <span class="tex-span">1</span>.</li><li> If he chooses elements <span class="tex-span">5</span> and <span class="tex-span">4</span>, then Limak is able to transform <span class="tex-span">5</span> into <span class="tex-span">6</span>, <span class="tex-span">6</span> into <span class="tex-span">3</span>, <span class="tex-span">3</span> into <span class="tex-span">4</span> (half way already behind him), <span class="tex-span">4</span> into <span class="tex-span">2</span>, <span class="tex-span">2</span> into <span class="tex-span">1</span>, <span class="tex-span">1</span> into <span class="tex-span">5</span>.</li><li> If he chooses elements <span class="tex-span">1</span> and <span class="tex-span">4</span>, then Limak is able to transform <span class="tex-span">1</span> into <span class="tex-span">2</span>, <span class="tex-span">2</span> into <span class="tex-span">4</span>, <span class="tex-span">4</span> into <span class="tex-span">3</span>, <span class="tex-span">3</span> into <span class="tex-span">6</span>, <span class="tex-span">6</span> into <span class="tex-span">5</span> and <span class="tex-span">5</span> into <span class="tex-span">1</span>. </li></ul><p>So Limak is able to execute task. Answer is "<span class="tex-font-style-tt">YES</span>" and <span class="tex-span"><i>R</i></span> is increased by <span class="tex-span">3</span> (it's equal to <span class="tex-span">4</span> now).</p><p>In last gossip <span class="tex-span">{1, 2}</span> and <span class="tex-span">(1, 2)</span> are deciphered to be <span class="tex-span">{5, 6}</span> and <span class="tex-span">(5, 6)</span>. Now there are <span class="tex-span">2</span> machines <span class="tex-span">(5, 6)</span> so Limak is able to execute task again.</p>
