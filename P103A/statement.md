## Description

<div><p>The average miner Vaganych took refresher courses. As soon as a miner completes the courses, he should take exams. The hardest one is a computer test called "Testing Pants for Sadness".</p><p>The test consists of <span class="tex-span"><i>n</i></span> questions; the questions are to be answered strictly in the order in which they are given, from question <span class="tex-span">1</span> to question <span class="tex-span"><i>n</i></span>. Question <span class="tex-span"><i>i</i></span> contains <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> answer variants, exactly one of them is correct. </p><p>A click is regarded as selecting any answer in any question. The goal is to select the correct answer for each of the <span class="tex-span"><i>n</i></span> questions. If Vaganych selects a wrong answer for some question, then all selected answers become unselected and the test starts from the very beginning, from question <span class="tex-span">1</span> again. But Vaganych remembers everything. The order of answers for each question and the order of questions remain unchanged, as well as the question and answers themselves.</p><p>Vaganych is very smart and his memory is superb, yet he is unbelievably unlucky and knows nothing whatsoever about the test's theme. How many clicks will he have to perform in the worst case?</p></div><div class="input-specification"><p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). It is the number of questions in the test. The second line contains space-separated <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the number of answer variants to question <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Print a single number — the minimal number of clicks needed to pass the test it the worst-case scenario. </p><p>Please do not use the %lld specificator to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the %I64d specificator.</p></div>

## Input

<p>The first line contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). It is the number of questions in the test. The second line contains space-separated <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the number of answer variants to question <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Print a single number — the minimal number of clicks needed to pass the test it the worst-case scenario. </p><p>Please do not use the %lld specificator to read or write 64-bit integers in С++. It is preferred to use the cin, cout streams or the %I64d specificator.</p>





```input1
2
1 1

```




```input2
2
2 2

```




```input3
1
10

```




```output1
2
```




```output2
5
```




```output3
10
```



## Note

<p>Note to the second sample. In the worst-case scenario you will need five clicks: </p><ul> <li> the first click selects the first variant to the first question, this answer turns out to be wrong. </li><li> the second click selects the second variant to the first question, it proves correct and we move on to the second question; </li><li> the third click selects the first variant to the second question, it is wrong and we go back to question 1; </li><li> the fourth click selects the second variant to the first question, it proves as correct as it was and we move on to the second question; </li><li> the fifth click selects the second variant to the second question, it proves correct, the test is finished. </li></ul>
