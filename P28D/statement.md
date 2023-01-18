## Description

<div><p>A motorcade of <span class="tex-span"><i>n</i></span> trucks, driving from city «Z» to city «З», has approached a tunnel, known as Tunnel of Horror. Among truck drivers there were rumours about monster DravDe, who hunts for drivers in that tunnel. Some drivers fear to go first, others - to be the last, but let's consider the general case. Each truck is described with four numbers: </p><ul> <li> <span class="tex-span"><i>v</i></span> — value of the truck, of its passangers and cargo </li><li> <span class="tex-span"><i>c</i></span> — amount of passanger on the truck, the driver included </li><li> <span class="tex-span"><i>l</i></span> — total amount of people that should go into the tunnel before this truck, so that the driver can overcome his fear («if the monster appears in front of the motorcade, he'll eat them first») </li><li> <span class="tex-span"><i>r</i></span> — total amount of people that should follow this truck, so that the driver can overcome his fear («if the monster appears behind the motorcade, he'll eat them first»). </li></ul><p>Since the road is narrow, it's impossible to escape DravDe, if he appears from one side. Moreover, the motorcade can't be rearranged. The order of the trucks can't be changed, but it's possible to take any truck out of the motorcade, and leave it near the tunnel for an indefinite period. You, as the head of the motorcade, should remove some of the trucks so, that the rest of the motorcade can move into the tunnel and the total amount of the left trucks' values is maximal. </p></div><div class="input-specification"><p>The first input line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — amount of trucks in the motorcade. The following <span class="tex-span"><i>n</i></span> lines contain four integers each. Numbers in the <span class="tex-span"><i>i</i></span>-th line: <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — describe the <span class="tex-span"><i>i</i></span>-th truck. The trucks are numbered from 1, counting from the front of the motorcade.</p></div><div class="output-specification"><p>In the first line output number <span class="tex-span"><i>k</i></span> — amount of trucks that will drive into the tunnel. In the second line output <span class="tex-span"><i>k</i></span> numbers — indexes of these trucks in ascending order. Don't forget please that you are not allowed to change the order of trucks. If the answer is not unique, output any.</p></div>

## Input

<p>The first input line contains integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — amount of trucks in the motorcade. The following <span class="tex-span"><i>n</i></span> lines contain four integers each. Numbers in the <span class="tex-span"><i>i</i></span>-th line: <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>, 1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>, 0 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — describe the <span class="tex-span"><i>i</i></span>-th truck. The trucks are numbered from 1, counting from the front of the motorcade.</p>

## Output

<p>In the first line output number <span class="tex-span"><i>k</i></span> — amount of trucks that will drive into the tunnel. In the second line output <span class="tex-span"><i>k</i></span> numbers — indexes of these trucks in ascending order. Don't forget please that you are not allowed to change the order of trucks. If the answer is not unique, output any.</p>





```input1
5
1 1 0 3
1 1 1 2
1 1 2 1
1 1 3 0
2 1 3 0

```




```input2
5
1 1 0 3
10 1 2 1
2 2 1 1
10 1 1 2
3 1 3 0

```




```output1
4
1 2 3 5 

```




```output2
3
1 3 5 

```


