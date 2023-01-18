## Description

<div><p>Each month Blake gets the report containing main economic indicators of the company "Blake Technologies". There are <span class="tex-span"><i>n</i></span> commodities produced by the company. For each of them there is exactly one integer in the final report, that denotes corresponding revenue. Before the report gets to Blake, it passes through the hands of <span class="tex-span"><i>m</i></span> managers. Each of them may reorder the elements in some order. Namely, the <span class="tex-span"><i>i</i></span>-th manager either sorts first <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> numbers in non-descending or non-ascending order and then passes the report to the manager <span class="tex-span"><i>i</i> + 1</span>, or directly to Blake (if this manager has number <span class="tex-span"><i>i</i> = <i>m</i></span>).</p><p>Employees of the "Blake Technologies" are preparing the report right now. You know the initial sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of length <span class="tex-span"><i>n</i></span> and the description of each manager, that is value <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> and his favourite order. You are asked to speed up the process and determine how the final report will look like.</p></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 200 000</span>)&nbsp;— the number of commodities in the report and the number of managers, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the initial report before it gets to the first manager.</p><p>Then follow <span class="tex-span"><i>m</i></span> lines with the descriptions of the operations managers are going to perform. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://n70USkZn.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), meaning that the <span class="tex-span"><i>i</i></span>-th manager sorts the first <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> numbers either in the non-descending (if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>) or non-ascending (if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>) order.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> integers&nbsp;— the final report, which will be passed to Blake by manager number <span class="tex-span"><i>m</i></span>.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 200 000</span>)&nbsp;— the number of commodities in the report and the number of managers, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the initial report before it gets to the first manager.</p><p>Then follow <span class="tex-span"><i>m</i></span> lines with the descriptions of the operations managers are going to perform. The <span class="tex-span"><i>i</i></span>-th of these lines contains two integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<img align="middle" class="tex-formula" src="file://n70USkZn.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), meaning that the <span class="tex-span"><i>i</i></span>-th manager sorts the first <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> numbers either in the non-descending (if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 1</span>) or non-ascending (if <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> = 2</span>) order.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> integers&nbsp;— the final report, which will be passed to Blake by manager number <span class="tex-span"><i>m</i></span>.</p>





```input1
3 1
1 2 3
2 2

```




```input2
4 2
1 2 4 3
2 3
1 2

```




```output1
2 1 3
```




```output2
2 4 1 3
```



## Note

<p>In the first sample, the initial report looked like: <span class="tex-font-style-tt">1 2 3</span>. After the first manager the first two numbers were transposed: <span class="tex-font-style-tt"><span class="tex-font-style-bf">2 1</span> 3</span>. The report got to Blake in this form.</p><p>In the second sample the original report was like this: <span class="tex-font-style-tt">1 2 4 3</span>. After the first manager the report changed to: <span class="tex-font-style-tt"><span class="tex-font-style-bf">4 2 1</span> 3</span>. After the second manager the report changed to: <span class="tex-font-style-tt"><span class="tex-font-style-bf">2 4</span> 1 3</span>. This report was handed over to Blake.</p>
