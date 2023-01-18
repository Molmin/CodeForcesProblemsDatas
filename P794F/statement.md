## Description

<div><p>Bankopolis, the city you already know, finally got a new bank opened! Unfortunately, its security system is not yet working fine... Meanwhile hacker Leha arrived in Bankopolis and decided to test the system!</p><p>Bank has <span class="tex-span"><i>n</i></span> cells for clients' money. A sequence from <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> describes the amount of money each client has. Leha wants to make requests to the database of the bank, finding out the total amount of money on some subsegments of the sequence and changing values of the sequence on some subsegments. Using a bug in the system, Leha can requests two types of queries to the database:</p><ul> <li> <span class="tex-font-style-tt">1 l r x y</span> denoting that Leha changes each digit <span class="tex-span"><i>x</i></span> to digit <span class="tex-span"><i>y</i></span> in each element of sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, for which <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> is holds. For example, if we change in number <span class="tex-span">11984381</span> digit <span class="tex-span">8</span> to <span class="tex-span">4</span>, we get <span class="tex-span">11944341</span>. It's worth noting that Leha, in order to stay in the shadow, never changes digits in the database to <span class="tex-span">0</span>, i.e. <span class="tex-span"><i>y</i> ≠ 0</span>. </li><li> <span class="tex-font-style-tt">2 l r</span> denoting that Leha asks to calculate and print the sum of such elements of sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, for which <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> holds. </li></ul><p>As Leha is a white-hat hacker, he don't want to test this vulnerability on a real database. You are to write a similar database for Leha to test.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) denoting amount of cells in the bank and total amount of queries respectively. </p><p>The following line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">9</sup></span>) denoting the amount of money in each cell initially. These integers do not contain leading zeros.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines has one of the formats:</p><ul> <li> <span class="tex-font-style-tt">1 l r x y</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 9</span>, <span class="tex-span">1 ≤ <i>y</i> ≤ 9</span>), denoting Leha asks to change each digit <span class="tex-span"><i>x</i></span> on digit <span class="tex-span"><i>y</i></span> for each element <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of the sequence for which <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> holds; </li><li> <span class="tex-font-style-tt">2 l r</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>), denoting you have to calculate and print the sum of elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> for which <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> holds. </li></ul></div><div class="output-specification"><p>For each second type query print a single number denoting the required sum.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) denoting amount of cells in the bank and total amount of queries respectively. </p><p>The following line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">9</sup></span>) denoting the amount of money in each cell initially. These integers do not contain leading zeros.</p><p>Each of the following <span class="tex-span"><i>q</i></span> lines has one of the formats:</p><ul> <li> <span class="tex-font-style-tt">1 l r x y</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 9</span>, <span class="tex-span">1 ≤ <i>y</i> ≤ 9</span>), denoting Leha asks to change each digit <span class="tex-span"><i>x</i></span> on digit <span class="tex-span"><i>y</i></span> for each element <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of the sequence for which <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> holds; </li><li> <span class="tex-font-style-tt">2 l r</span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>), denoting you have to calculate and print the sum of elements <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> for which <span class="tex-span"><i>l</i> ≤ <i>i</i> ≤ <i>r</i></span> holds. </li></ul>

## Output

<p>For each second type query print a single number denoting the required sum.</p>





```input1
5 5
38 43 4 12 70
1 1 3 4 8
2 2 4
1 4 5 0 8
1 2 5 8 7
2 1 5

```




```input2
5 5
25 36 39 40 899
1 1 3 2 7
2 1 2
1 3 5 9 1
1 4 4 0 9
2 1 5

```




```output1
103
207

```




```output2
111
1002

```



## Note

<p>Let's look at the example testcase.</p><p>Initially the sequence is <span class="tex-span">[38, 43, 4, 12, 70]</span>. </p><p>After the first change each digit equal to <span class="tex-span">4</span> becomes <span class="tex-span">8</span> for each element with index in interval <span class="tex-span">[1;&nbsp;3]</span>. Thus, the new sequence is <span class="tex-span">[38, 83, 8, 12, 70]</span>.</p><p>The answer for the first sum's query is the sum in the interval <span class="tex-span">[2;&nbsp;4]</span>, which equal <span class="tex-span">83 + 8 + 12 = 103</span>, so the answer to this query is <span class="tex-span">103</span>.</p><p>The sequence becomes <span class="tex-span">[38, 83, 8, 12, 78]</span> after the second change and <span class="tex-span">[38, 73, 7, 12, 77]</span> after the third.</p><p>The answer for the second sum's query is <span class="tex-span">38 + 73 + 7 + 12 + 77 = 207</span>.</p>
