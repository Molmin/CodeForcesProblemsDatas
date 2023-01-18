## Description

<div><p>There are several days left before the fiftieth birthday of a famous Berland's writer Berlbury. In this connection the local library decided to make an exposition of the works of this famous science-fiction writer. It was decided as well that it is necessary to include into the exposition only those books that were published during a particular time period. It is obvious that if the books differ much in size, the visitors will not like it. That was why the organizers came to the opinion, that the difference between the highest and the lowest books in the exposition should be not more than <span class="tex-span"><i>k</i></span> millimeters.</p><p>The library has <span class="tex-span"><i>n</i></span> volumes of books by Berlbury, arranged in chronological order of their appearance. The height of each book in millimeters is know, it is <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. As Berlbury is highly respected in the city, the organizers want to include into the exposition as many books as possible, and to find out what periods of his creative work they will manage to cover. You are asked to help the organizers cope with this hard task.</p></div><div class="input-specification"><p>The first line of the input data contains two integer numbers separated by a space <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>) — the amount of books by Berlbury in the library, and the maximum allowed height difference between the lowest and the highest books. The second line contains <span class="tex-span"><i>n</i></span> integer numbers separated by a space. Each number <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) is the height of the <span class="tex-span"><i>i</i></span>-th book in millimeters.</p></div><div class="output-specification"><p>In the first line of the output data print two numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (separate them by a space), where <span class="tex-span"><i>a</i></span> is the maximum amount of books the organizers can include into the exposition, and <span class="tex-span"><i>b</i></span> — the amount of the time periods, during which Berlbury published <span class="tex-span"><i>a</i></span> books, and the height difference between the lowest and the highest among these books is not more than <span class="tex-span"><i>k</i></span> milllimeters.</p><p>In each of the following <span class="tex-span"><i>b</i></span> lines print two integer numbers separated by a space — indexes of the first and the last volumes from each of the required time periods of Berlbury's creative work.</p></div>

## Input

<p>The first line of the input data contains two integer numbers separated by a space <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>) — the amount of books by Berlbury in the library, and the maximum allowed height difference between the lowest and the highest books. The second line contains <span class="tex-span"><i>n</i></span> integer numbers separated by a space. Each number <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>) is the height of the <span class="tex-span"><i>i</i></span>-th book in millimeters.</p>

## Output

<p>In the first line of the output data print two numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (separate them by a space), where <span class="tex-span"><i>a</i></span> is the maximum amount of books the organizers can include into the exposition, and <span class="tex-span"><i>b</i></span> — the amount of the time periods, during which Berlbury published <span class="tex-span"><i>a</i></span> books, and the height difference between the lowest and the highest among these books is not more than <span class="tex-span"><i>k</i></span> milllimeters.</p><p>In each of the following <span class="tex-span"><i>b</i></span> lines print two integer numbers separated by a space — indexes of the first and the last volumes from each of the required time periods of Berlbury's creative work.</p>





```input1
3 3
14 12 10

```




```input2
2 0
10 10

```




```input3
4 5
8 19 10 13

```




```output1
2 2
1 2
2 3

```




```output2
2 1
1 2

```




```output3
2 1
3 4

```


