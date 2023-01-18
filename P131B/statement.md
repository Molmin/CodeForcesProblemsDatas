## Description

<div><p>Everybody knows that opposites attract. That is the key principle of the "Perfect Matching" dating agency. The "Perfect Matching" matchmakers have classified each registered customer by his interests and assigned to the <span class="tex-span"><i>i</i></span>-th client number <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>). Of course, one number can be assigned to any number of customers.</p><p>"Perfect Matching" wants to advertise its services and publish the number of opposite couples, that is, the couples who have opposite values of <span class="tex-span"><i>t</i></span>. Each couple consists of exactly two clients. The customer can be included in a couple an arbitrary number of times. Help the agency and write the program that will find the sought number by the given sequence <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>. For example, if <span class="tex-span"><i>t</i> = (1,  - 1, 1,  - 1)</span>, then any two elements <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index"><i>j</i></sub></span> form a couple if <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> have different parity. Consequently, in this case the sought number equals 4.</p><p>Of course, a client can't form a couple with him/herself.</p></div><div class="input-specification"><p>The first line of the input data contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) which represents the number of registered clients of the "Couple Matching". The second line contains a sequence of integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>), <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — is the parameter of the <span class="tex-span"><i>i</i></span>-th customer that has been assigned to the customer by the result of the analysis of his interests.</p></div><div class="output-specification"><p>Print the number of couples of customs with opposite <span class="tex-span"><i>t</i></span>. The opposite number for <span class="tex-span"><i>x</i></span> is number <span class="tex-span"> - <i>x</i></span> (<span class="tex-span">0</span> is opposite to itself). Couples that only differ in the clients' order are considered the same.</p><p>Note that the answer to the problem can be large enough, so you must use the 64-bit integer type for calculations. Please, do not use the %lld specificator to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the %I64d specificator.</p></div>

## Input

<p>The first line of the input data contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) which represents the number of registered clients of the "Couple Matching". The second line contains a sequence of integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10</span>), <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — is the parameter of the <span class="tex-span"><i>i</i></span>-th customer that has been assigned to the customer by the result of the analysis of his interests.</p>

## Output

<p>Print the number of couples of customs with opposite <span class="tex-span"><i>t</i></span>. The opposite number for <span class="tex-span"><i>x</i></span> is number <span class="tex-span"> - <i>x</i></span> (<span class="tex-span">0</span> is opposite to itself). Couples that only differ in the clients' order are considered the same.</p><p>Note that the answer to the problem can be large enough, so you must use the 64-bit integer type for calculations. Please, do not use the %lld specificator to read or write 64-bit integers in С++. It is preferred to use cin, cout streams or the %I64d specificator.</p>





```input1
5
-3 3 0 0 3

```




```input2
3
0 0 0

```




```output1
3

```




```output2
3

```



## Note

<p>In the first sample the couples of opposite clients are: <span class="tex-font-style-bf">(1,2), (1,5) и (3,4)</span>.</p><p>In the second sample any couple of clients is opposite.</p>
