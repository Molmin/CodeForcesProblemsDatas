## Description

<div><p>Once <span class="tex-span"><i>n</i></span> people simultaneously signed in to the reception at the recently opened, but already thoroughly bureaucratic organization (abbreviated TBO). As the organization is thoroughly bureaucratic, it can accept and cater for exactly one person per day. As a consequence, each of <span class="tex-span"><i>n</i></span> people made an appointment on one of the next <span class="tex-span"><i>n</i></span> days, and no two persons have an appointment on the same day.</p><p>However, the organization workers are very irresponsible about their job, so none of the signed in people was told the exact date of the appointment. The only way to know when people should come is to write some requests to TBO.</p><p>The request form consists of <span class="tex-span"><i>m</i></span> empty lines. Into each of these lines the name of a signed in person can be written (it can be left blank as well). Writing a person's name in the same form twice is forbidden, such requests are ignored. TBO responds very quickly to written requests, but the reply format is of very poor quality — that is, the response contains the correct appointment dates for all people from the request form, but the dates are in completely random order. Responds to all requests arrive simultaneously at the end of the day (each response specifies the request that it answers).</p><p>Fortunately, you aren't among these <span class="tex-span"><i>n</i></span> lucky guys. As an observer, you have the following task — given <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span>, determine the minimum number of requests to submit to TBO to clearly determine the appointment date for each person.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 1000</span>) — the number of test cases. Each of the following <span class="tex-span"><i>t</i></span> lines contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of people who have got an appointment at TBO and the number of empty lines in the request form, correspondingly.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>t</i></span> lines, each containing an answer for the corresponding test case (in the order they are given in the input) — the minimum number of requests to submit to TBO.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 1000</span>) — the number of test cases. Each of the following <span class="tex-span"><i>t</i></span> lines contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">9</sup></span>) — the number of people who have got an appointment at TBO and the number of empty lines in the request form, correspondingly.</p>

## Output

<p>Print <span class="tex-span"><i>t</i></span> lines, each containing an answer for the corresponding test case (in the order they are given in the input) — the minimum number of requests to submit to TBO.</p>





```input1
5
4 1
4 2
7 3
1 1
42 7

```




```output1
3
2
3
0
11

```



## Note

<p>In the first sample, you need to submit three requests to TBO with three different names. When you learn the appointment dates of three people out of four, you can find out the fourth person's date by elimination, so you do not need a fourth request.</p><p>In the second sample you need only two requests. Let's number the persons from <span class="tex-span">1</span> to <span class="tex-span">4</span> and mention persons <span class="tex-span">1</span> and <span class="tex-span">2</span> in the first request and persons <span class="tex-span">1</span> and <span class="tex-span">3</span> in the second request. It is easy to see that after that we can clearly determine each person's appointment date regardless of the answers obtained from TBO.</p><p>In the fourth sample only one person signed up for an appointment. He doesn't need to submit any requests — his appointment date is tomorrow.</p>
