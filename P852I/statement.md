## Description

<div><p>This story is happening in a town named BubbleLand. There are <span class="tex-span"><i>n</i></span> houses in BubbleLand. In each of these <span class="tex-span"><i>n</i></span> houses lives a boy or a girl. People there really love numbers and everyone has their favorite number <span class="tex-span"><i>f</i></span>. That means that the boy or girl that lives in the <span class="tex-span"><i>i</i></span>-th house has favorite number equal to <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The houses are numerated with numbers <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>The houses are connected with <span class="tex-span"><i>n</i> - 1</span> bidirectional roads and you can travel from any house to any other house in the town. There is exactly one path between every pair of houses.</p><p>A new dating had agency opened their offices in this mysterious town and the citizens were very excited. They immediately sent <span class="tex-span"><i>q</i></span> questions to the agency and each question was of the following format: </p><ul> <li> <span class="tex-span"><i>a</i> <i>b</i></span>&nbsp;— asking how many ways are there to choose a couple (boy and girl) that have the same favorite number and live in one of the houses on the unique path from house <span class="tex-span"><i>a</i></span> to house <span class="tex-span"><i>b</i></span>. </li></ul><p>Help the dating agency to answer the questions and grow their business.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of houses in the town.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th number is <span class="tex-span">1</span> if a boy lives in the <span class="tex-span"><i>i</i></span>-th house or <span class="tex-span">0</span> if a girl lives in <span class="tex-span"><i>i</i></span>-th house.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th number represents the favorite number <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) of the girl or boy that lives in the <span class="tex-span"><i>i</i></span>-th house.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain information about the roads and the <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) which means that there exists road between those two houses. It is guaranteed that it's possible to reach any house from any other.</p><p>The following line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of queries.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines represents a question and consists of two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>For each of the <span class="tex-span"><i>q</i></span> questions output a single number, the answer to the citizens question.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of houses in the town.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th number is <span class="tex-span">1</span> if a boy lives in the <span class="tex-span"><i>i</i></span>-th house or <span class="tex-span">0</span> if a girl lives in <span class="tex-span"><i>i</i></span>-th house.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers, where the <span class="tex-span"><i>i</i></span>-th number represents the favorite number <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) of the girl or boy that lives in the <span class="tex-span"><i>i</i></span>-th house.</p><p>The next <span class="tex-span"><i>n</i> - 1</span> lines contain information about the roads and the <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) which means that there exists road between those two houses. It is guaranteed that it's possible to reach any house from any other.</p><p>The following line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>), the number of queries.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines represents a question and consists of two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>).</p>

## Output

<p>For each of the <span class="tex-span"><i>q</i></span> questions output a single number, the answer to the citizens question.</p>





```input1
7
1 0 0 1 0 1 0
9 2 9 2 2 9 9
2 6
1 2
4 2
6 5
3 6
7 4
2
1 3
7 5

```




```output1
2
3

```



## Note

<p>In the first question from house <span class="tex-span">1</span> to house <span class="tex-span">3</span>, the potential couples are <span class="tex-span">(1, 3)</span> and <span class="tex-span">(6, 3)</span>.</p><p>In the second question from house <span class="tex-span">7</span> to house <span class="tex-span">5</span>, the potential couples are <span class="tex-span">(7, 6)</span>, <span class="tex-span">(4, 2)</span> and <span class="tex-span">(4, 5)</span>.</p>
