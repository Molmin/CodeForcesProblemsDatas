## Description

<div><p>BigData Inc. is a corporation that has <span class="tex-span"><i>n</i></span> data centers indexed from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> that are located all over the world. These data centers provide storage for client data (you can figure out that client data is really big!).</p><p>Main feature of services offered by BigData Inc. is the access availability guarantee even under the circumstances of any data center having an outage. Such a guarantee is ensured by using the <span class="tex-font-style-it">two-way replication</span>. Two-way replication is such an approach for data storage that any piece of data is represented by two identical copies that are stored in two different data centers.</p><p>For each of <span class="tex-span"><i>m</i></span> company clients, let us denote indices of two different data centers storing this client data as <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, 1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, 2</sub></span>.</p><p>In order to keep data centers operational and safe, the software running on data center computers is being updated regularly. Release cycle of BigData Inc. is one day meaning that the new version of software is being deployed to the data center computers each day.</p><p>Data center software update is a non-trivial long process, that is why there is a special hour-long time frame that is dedicated for data center maintenance. During the maintenance period, data center computers are installing software updates, and thus they may be unavailable. Consider the day to be exactly <span class="tex-span"><i>h</i></span> hours long. For each data center there is an integer <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">0 ≤ <i>u</i><sub class="lower-index"><i>j</i></sub> ≤ <i>h</i> - 1</span>) defining the index of an hour of day, such that during this hour data center <span class="tex-span"><i>j</i></span> is unavailable due to maintenance.</p><p>Summing up everything above, the condition <span class="tex-span"><i>u</i><sub class="lower-index"><i>c</i><sub class="lower-index"><i>i</i>, 1</sub></sub> ≠ <i>u</i><sub class="lower-index"><i>c</i><sub class="lower-index"><i>i</i>, 2</sub></sub></span> should hold for each client, or otherwise his data may be unaccessible while data centers that store it are under maintenance.</p><p>Due to occasional timezone change in different cities all over the world, the maintenance time in some of the data centers may change by one hour sometimes. Company should be prepared for such situation, that is why they decided to conduct an experiment, choosing some non-empty subset of data centers, and shifting the maintenance time for them by an hour later (i.e. if <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub> = <i>h</i> - 1</span>, then the new maintenance hour would become <span class="tex-span">0</span>, otherwise it would become <span class="tex-span"><i>u</i><sub class="lower-index"><i>j</i></sub> + 1</span>). Nonetheless, such an experiment should not break the accessibility guarantees, meaning that data of any client should be still available during any hour of a day after the data center maintenance times are changed.</p><p>Such an experiment would provide useful insights, but changing update time is quite an expensive procedure, that is why the company asked you to find out the minimum number of data centers that have to be included in an experiment in order to keep the data accessibility guarantees.</p></div><div class="input-specification"><p>The first line of input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>, <span class="tex-span">2 ≤ <i>h</i> ≤ 100 000</span>), the number of company data centers, number of clients and the day length of day measured in hours. </p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>u</i><sub class="lower-index">1</sub>, <i>u</i><sub class="lower-index">2</sub>, ..., <i>u</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>u</i><sub class="lower-index"><i>j</i></sub> &lt; <i>h</i></span>), <span class="tex-span"><i>j</i></span>-th of these numbers is an index of a maintenance hour for data center <span class="tex-span"><i>j</i></span>. </p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, 1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, 2</sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>c</i><sub class="lower-index"><i>i</i>, 2</sub> ≤ <i>n</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, 1</sub> ≠ <i>c</i><sub class="lower-index"><i>i</i>, 2</sub></span>), defining the data center indices containing the data of client <span class="tex-span"><i>i</i></span>.</p><p>It is guaranteed that the given maintenance schedule allows each client to access at least one copy of his data at any moment of day.</p></div><div class="output-specification"><p>In the first line print the minimum possible number of data centers <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>) that have to be included in an experiment in order to keep the data available for any client.</p><p>In the second line print <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), the indices of data centers whose maintenance time will be shifted by one hour later. Data center indices may be printed in any order.</p><p>If there are several possible answers, it is allowed to print any of them. It is guaranteed that at there is at least one valid choice of data centers.</p></div>

## Input

<p>The first line of input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100 000</span>, <span class="tex-span">2 ≤ <i>h</i> ≤ 100 000</span>), the number of company data centers, number of clients and the day length of day measured in hours. </p><p>The second line of input contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>u</i><sub class="lower-index">1</sub>, <i>u</i><sub class="lower-index">2</sub>, ..., <i>u</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>u</i><sub class="lower-index"><i>j</i></sub> &lt; <i>h</i></span>), <span class="tex-span"><i>j</i></span>-th of these numbers is an index of a maintenance hour for data center <span class="tex-span"><i>j</i></span>. </p><p>Each of the next <span class="tex-span"><i>m</i></span> lines contains two integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, 1</sub></span> and <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, 2</sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>c</i><sub class="lower-index"><i>i</i>, 2</sub> ≤ <i>n</i></span>, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i>, 1</sub> ≠ <i>c</i><sub class="lower-index"><i>i</i>, 2</sub></span>), defining the data center indices containing the data of client <span class="tex-span"><i>i</i></span>.</p><p>It is guaranteed that the given maintenance schedule allows each client to access at least one copy of his data at any moment of day.</p>

## Output

<p>In the first line print the minimum possible number of data centers <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>) that have to be included in an experiment in order to keep the data available for any client.</p><p>In the second line print <span class="tex-span"><i>k</i></span> distinct integers <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ..., <i>x</i><sub class="lower-index"><i>k</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), the indices of data centers whose maintenance time will be shifted by one hour later. Data center indices may be printed in any order.</p><p>If there are several possible answers, it is allowed to print any of them. It is guaranteed that at there is at least one valid choice of data centers.</p>





```input1
3 3 5
4 4 0
1 3
3 2
3 1

```




```input2
4 5 4
2 1 0 3
4 3
3 2
1 2
1 4
1 3

```




```output1
1
3
```




```output2
4
1 2 3 4
```



## Note

<p>Consider the first sample test. The given answer is the only way to conduct an experiment involving the only data center. In such a scenario the third data center has a maintenance during the hour 1, and no two data centers storing the information of the same client have maintenance at the same hour.</p><p>On the other hand, for example, if we shift the maintenance time on hour later for the first data center, then the data of clients 1 and 3 will be unavailable during the hour 0.</p>
