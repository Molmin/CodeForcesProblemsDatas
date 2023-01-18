## Description

<div><p>Do you know the story about the three musketeers? Anyway, you must help them now.</p><p>Richelimakieu is a cardinal in the city of Bearis. He found three brave warriors and called them the three musketeers. Athos has strength <span class="tex-span"><i>a</i></span>, Borthos strength <span class="tex-span"><i>b</i></span>, and Caramis has strength <span class="tex-span"><i>c</i></span>.</p><p>The year 2015 is almost over and there are still <span class="tex-span"><i>n</i></span> criminals to be defeated. The <span class="tex-span"><i>i</i></span>-th criminal has strength <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>. It's hard to defeat strong criminals&nbsp;— maybe musketeers will have to fight together to achieve it.</p><p>Richelimakieu will coordinate musketeers' actions. In each hour each musketeer can either do nothing or be assigned to one criminal. Two or three musketeers can be assigned to the same criminal and then their strengths are summed up. A criminal can be defeated in exactly one hour (also if two or three musketeers fight him). Richelimakieu can't allow the situation where a criminal has strength bigger than the sum of strengths of musketeers fighting him&nbsp;— a criminal would win then!</p><p>In other words, there are three ways to defeat a criminal.</p><ul> <li> A musketeer of the strength <span class="tex-span"><i>x</i></span> in one hour can defeat a criminal of the strength not greater than <span class="tex-span"><i>x</i></span>. So, for example Athos in one hour can defeat criminal <span class="tex-span"><i>i</i></span> only if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i></span>. </li><li> Two musketeers can fight together and in one hour defeat a criminal of the strength not greater than the sum of strengths of these two musketeers. So, for example Athos and Caramis in one hour can defeat criminal <span class="tex-span"><i>i</i></span> only if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i> + <i>c</i></span>. Note that the third remaining musketeer can either do nothing or fight some other criminal. </li><li> Similarly, all three musketeers can fight together and in one hour defeat a criminal of the strength not greater than the sum of musketeers' strengths, i.e. <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> ≤ <i>a</i> + <i>b</i> + <i>c</i></span>. </li></ul><p>Richelimakieu doesn't want musketeers to fight during the New Year's Eve. Thus, he must coordinate their actions in order to minimize the number of hours till all criminals will be defeated.</p><p>Find the minimum number of hours to defeat all criminals. If musketeers can't defeat them all then print "<span class="tex-font-style-tt">-1</span>" (without the quotes) instead.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of criminals.</p><p>The second line contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— strengths of musketeers.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— strengths of criminals.</p></div><div class="output-specification"><p>Print one line with the answer.</p><p>If it's impossible to defeat all criminals, print "<span class="tex-font-style-tt">-1</span>" (without the quotes). Otherwise, print the minimum number of hours the three musketeers will spend on defeating all criminals.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of criminals.</p><p>The second line contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— strengths of musketeers.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">8</sup></span>)&nbsp;— strengths of criminals.</p>

## Output

<p>Print one line with the answer.</p><p>If it's impossible to defeat all criminals, print "<span class="tex-font-style-tt">-1</span>" (without the quotes). Otherwise, print the minimum number of hours the three musketeers will spend on defeating all criminals.</p>





```input1
5
10 20 30
1 1 1 1 50

```




```input2
5
10 20 30
1 1 1 1 51

```




```input3
7
30 20 10
34 19 50 33 88 15 20

```




```input4
6
10 5 10
10 9 5 25 20 5

```




```output1
2

```




```output2
3

```




```output3
-1

```




```output4
3

```



## Note

<p>In the first sample Athos has strength <span class="tex-span">10</span>, Borthos <span class="tex-span">20</span>, and Caramis <span class="tex-span">30</span>. They can defeat all criminals in two hours:</p><ul> <li> Borthos and Caramis should together fight a criminal with strength <span class="tex-span">50</span>. In the same hour Athos can fight one of four criminals with strength <span class="tex-span">1</span>. </li><li> There are three criminals left, each with strength <span class="tex-span">1</span>. Each musketeer can fight one criminal in the second hour. </li></ul> <p>In the second sample all three musketeers must together fight a criminal with strength <span class="tex-span">51</span>. It takes one hour. In the second hour they can fight separately, each with one criminal. In the third hour one criminal is left and any of musketeers can fight him.</p>
