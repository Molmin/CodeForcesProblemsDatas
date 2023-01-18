## Description

<div><p>As it has been found out recently, all the Berland's current economical state can be described using a simple table <span class="tex-span"><i>n</i> × <i>m</i></span> in size. <span class="tex-span"><i>n</i></span> — the number of days in each Berland month, <span class="tex-span"><i>m</i></span> — the number of months. Thus, a table cell corresponds to a day and a month of the Berland's year. Each cell will contain either <span class="tex-font-style-tt">1</span>, or <span class="tex-font-style-tt">-1</span>, which means the state's gains in a particular month, on a particular day. <span class="tex-font-style-tt">1</span> corresponds to profits, <span class="tex-font-style-tt">-1</span> corresponds to losses. It turned out important for successful development to analyze the data on the state of the economy of the previous year, however when the treasurers referred to the archives to retrieve the data, it turned out that the table had been substantially damaged. In some table cells the number values had faded and were impossible to be deciphered. It is known that the number of cells in which the data had been preserved is strictly less than <span class="tex-span"><i>max</i>(<i>n</i>, <i>m</i>)</span>. However, there is additional information — the product of the numbers in each line and column equaled <span class="tex-font-style-tt">-1</span>. Your task is to find out how many different tables may conform to the preserved data. As the answer to the task can be quite large, you have to find it modulo <span class="tex-span"><i>p</i></span>.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>). The second line contains the integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> &lt; <i>max</i>(<i>n</i>, <i>m</i>)</span>) — the number of cells in which the data had been preserved. The next <span class="tex-span"><i>k</i></span> lines contain the data on the state of the table in the preserved cells. Each line is of the form "<span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span> <span class="tex-span"><i>c</i></span>", where <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i></span>) — the number of the table row, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ <i>m</i></span>) — the number of the column, <span class="tex-span"><i>c</i></span> — the value containing in the cell (<span class="tex-font-style-tt">1</span> or <span class="tex-font-style-tt">-1</span>). They are numbered starting from <span class="tex-span">1</span>. It is guaranteed that no two lines with same <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> values exist. The last line contains an integer <span class="tex-span"><i>p</i></span> (<span class="tex-span">2 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="output-specification"><p>Print the number of different tables that could conform to the preserved data modulo <span class="tex-span"><i>p</i></span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 1000</span>). The second line contains the integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> &lt; <i>max</i>(<i>n</i>, <i>m</i>)</span>) — the number of cells in which the data had been preserved. The next <span class="tex-span"><i>k</i></span> lines contain the data on the state of the table in the preserved cells. Each line is of the form "<span class="tex-span"><i>a</i></span> <span class="tex-span"><i>b</i></span> <span class="tex-span"><i>c</i></span>", where <span class="tex-span"><i>a</i></span> (<span class="tex-span">1 ≤ <i>a</i> ≤ <i>n</i></span>) — the number of the table row, <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ <i>m</i></span>) — the number of the column, <span class="tex-span"><i>c</i></span> — the value containing in the cell (<span class="tex-font-style-tt">1</span> or <span class="tex-font-style-tt">-1</span>). They are numbered starting from <span class="tex-span">1</span>. It is guaranteed that no two lines with same <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> values exist. The last line contains an integer <span class="tex-span"><i>p</i></span> (<span class="tex-span">2 ≤ <i>p</i> ≤ 10<sup class="upper-index">9</sup> + 7</span>).</p>

## Output

<p>Print the number of different tables that could conform to the preserved data modulo <span class="tex-span"><i>p</i></span>.</p>





```input1
2 2
0
100

```




```input2
2 2
1
1 1 -1
100

```




```output1
2

```




```output2
1

```


