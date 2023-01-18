## Description

<div><p>Byteland is trying to send a space mission onto the Bit-X planet. Their task is complicated by the fact that the orbit of the planet is regularly patrolled by Captain Bitonix, the leader of the space forces of Bit-X.</p><p>There are <span class="tex-span"><i>n</i></span> stations around Bit-X numbered clockwise from 1 to <span class="tex-span"><i>n</i></span>. The stations are evenly placed on a circular orbit, so the stations number <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> <span class="tex-span">(1 ≤ <i>i</i> &lt; <i>n</i>)</span>, and the stations number 1 and <span class="tex-span"><i>n</i></span>, are neighboring. The distance between every pair of adjacent stations is equal to <span class="tex-span"><i>m</i></span> space miles. To go on a patrol, Captain Bitonix jumps in his rocket at one of the stations and flies in a circle, covering a distance of at least one space mile, before finishing in some (perhaps the starting) station.</p><p>Bitonix' rocket moves by burning fuel tanks. After Bitonix attaches an <span class="tex-span"><i>x</i></span>-liter fuel tank and chooses the direction (clockwise or counter-clockwise), the rocket flies exactly <span class="tex-span"><i>x</i></span> space miles along a circular orbit in the chosen direction. Note that the rocket has no brakes; it is not possible for the rocket to stop before depleting a fuel tank.</p><p>For example, assume that <span class="tex-span"><i>n</i> = 3</span> and <span class="tex-span"><i>m</i> = 60</span> and Bitonix has fuel tanks with volumes of 10, 60, 90 and 100 liters. If Bitonix starts from station 1, uses the 100-liter fuel tank to go clockwise, then uses the 90-liter fuel tank to go clockwise, and then uses the 10-liter fuel tank to go counterclockwise, he will finish back at station 1. This constitutes a valid patrol. Note that Bitonix does not have to use all available fuel tanks. Another valid option for Bitonix in this example would be to simply use the 60-liter fuel tank to fly to either station 2 or 3.</p><p>However, if <span class="tex-span"><i>n</i></span> was equal to 3, <span class="tex-span"><i>m</i></span> was equal to 60 and the only fuel tanks available to Bitonix were one 10-liter tank and one 100-liter tank, he would have no way of completing a valid patrol (he wouldn't be able to finish any patrol exactly at the station).</p><p>The Byteland space agency wants to destroy some of Captain Bitonix' fuel tanks so that he cannot to complete any valid patrol. Find how many different subsets of the tanks the agency can destroy to prevent Captain Bitonix from completing a patrol and output the answer modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) — the number of stations, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 120</span>) — the distance between adjacent stations, and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10000</span>) — the number of fuel tanks owned by Captain Bitonix.</p><p>The second line of the input contains <span class="tex-span"><i>t</i></span> space-separated integers between <span class="tex-span">1</span> and <span class="tex-span">10<sup class="upper-index">9</sup></span>, inclusive — the volumes of Bitonix' fuel tanks.</p></div><div class="output-specification"><p>Output a single number — the number of distinct subsets of tanks that the Bytelandian space agency can destroy in order to prevent Captain Bitonix from completing a patrol, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 1000</span>) — the number of stations, <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 120</span>) — the distance between adjacent stations, and <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10000</span>) — the number of fuel tanks owned by Captain Bitonix.</p><p>The second line of the input contains <span class="tex-span"><i>t</i></span> space-separated integers between <span class="tex-span">1</span> and <span class="tex-span">10<sup class="upper-index">9</sup></span>, inclusive — the volumes of Bitonix' fuel tanks.</p>

## Output

<p>Output a single number — the number of distinct subsets of tanks that the Bytelandian space agency can destroy in order to prevent Captain Bitonix from completing a patrol, modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
7 6 5
5 4 12 6 5

```




```input2
3 60 2
10 100

```




```output1
6

```




```output2
4

```



## Note

<p>All the fuel tanks are distinct, even if some of them have the same capacity.</p>
