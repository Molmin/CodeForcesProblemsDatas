## Description

<div><p>Scientists of planet Olympia are conducting an experiment in mutation of primitive organisms. Genome of organism from this planet can be represented as a string of the first <span class="tex-span"><i>K</i></span> capital English letters. For each pair of types of genes they assigned <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span> — a risk of disease occurence in the organism provided that genes of these types are adjacent in the genome, where <span class="tex-span"><i>i</i></span> — the 1-based index of the first gene and <span class="tex-span"><i>j</i></span> — the index of the second gene. The gene 'A' has index 1, 'B' has index 2 and so on. For example, <span class="tex-span"><i>a</i><sub class="lower-index">3, 2</sub></span> stands for the risk of 'CB' fragment. Risk of disease occurence in the organism is equal to the sum of risks for each pair of adjacent genes in the genome.</p><p>Scientists have already obtained a base organism. Some new organisms can be obtained by mutation of this organism. Mutation involves removal of all genes of some particular types. Such removal increases the total risk of disease occurence additionally. For each type of genes scientists determined <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the increasement of the total risk of disease occurence provided by removal of all genes having type with index <span class="tex-span"><i>i</i></span>. For example, <span class="tex-span"><i>t</i><sub class="lower-index">4</sub></span> stands for the value of additional total risk increasement in case of removing all the 'D' genes.</p><p>Scientists want to find a number of different organisms that can be obtained from the given one which have the total risk of disease occurence not greater than <span class="tex-span"><i>T</i></span>. They can use only the process of mutation described above. Two organisms are considered different if strings representing their genomes are different. Genome should contain at least one gene.</p></div><div class="input-specification"><p>The first line of the input contains three integer numbers <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 200 000</span>) — length of the genome of base organism, <span class="tex-span"><i>K</i></span> (<span class="tex-span">1 ≤ <i>K</i> ≤ 22</span>) — the maximal index of gene type in the genome and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 2·10<sup class="upper-index">9</sup></span>) — maximal allowable risk of disease occurence. The second line contains the genome of the given organism. It is a string of the first <span class="tex-span"><i>K</i></span> capital English letters having length <span class="tex-span"><i>N</i></span>.</p><p>The third line contains <span class="tex-span"><i>K</i></span> numbers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>K</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is additional risk value of disease occurence provided by removing of all genes of the <span class="tex-span"><i>i</i></span>-th type.</p><p>The following <span class="tex-span"><i>K</i></span> lines contain the elements of the given matrix <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>K</i></span> numbers. The <span class="tex-span"><i>j</i></span>-th number of the <span class="tex-span"><i>i</i></span>-th line stands for a risk of disease occurence for the pair of genes, first of which corresponds to the <span class="tex-span"><i>i</i></span>-th letter and second of which corresponds to the <span class="tex-span"><i>j</i></span>-th letter. The given matrix is <span class="tex-font-style-bf">not</span> necessarily symmetrical.</p><p>All the numbers in the input are integer, non-negative and all of them except <span class="tex-span"><i>T</i></span> are not greater than <span class="tex-span">10<sup class="upper-index">9</sup></span>. It is guaranteed that the maximal possible risk of organism that can be obtained from the given organism is strictly smaller than <span class="tex-span">2<sup class="upper-index">31</sup></span>.</p></div><div class="output-specification"><p>Output the number of organisms that can be obtained from the base one and which have the total risk of disease occurence not greater than <span class="tex-span"><i>T</i></span>.</p></div>

## Input

<p>The first line of the input contains three integer numbers <span class="tex-span"><i>N</i></span> (<span class="tex-span">1 ≤ <i>N</i> ≤ 200 000</span>) — length of the genome of base organism, <span class="tex-span"><i>K</i></span> (<span class="tex-span">1 ≤ <i>K</i> ≤ 22</span>) — the maximal index of gene type in the genome and <span class="tex-span"><i>T</i></span> (<span class="tex-span">1 ≤ <i>T</i> ≤ 2·10<sup class="upper-index">9</sup></span>) — maximal allowable risk of disease occurence. The second line contains the genome of the given organism. It is a string of the first <span class="tex-span"><i>K</i></span> capital English letters having length <span class="tex-span"><i>N</i></span>.</p><p>The third line contains <span class="tex-span"><i>K</i></span> numbers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>K</i></sub></span>, where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> is additional risk value of disease occurence provided by removing of all genes of the <span class="tex-span"><i>i</i></span>-th type.</p><p>The following <span class="tex-span"><i>K</i></span> lines contain the elements of the given matrix <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i>, <i>j</i></sub></span>. The <span class="tex-span"><i>i</i></span>-th line contains <span class="tex-span"><i>K</i></span> numbers. The <span class="tex-span"><i>j</i></span>-th number of the <span class="tex-span"><i>i</i></span>-th line stands for a risk of disease occurence for the pair of genes, first of which corresponds to the <span class="tex-span"><i>i</i></span>-th letter and second of which corresponds to the <span class="tex-span"><i>j</i></span>-th letter. The given matrix is <span class="tex-font-style-bf">not</span> necessarily symmetrical.</p><p>All the numbers in the input are integer, non-negative and all of them except <span class="tex-span"><i>T</i></span> are not greater than <span class="tex-span">10<sup class="upper-index">9</sup></span>. It is guaranteed that the maximal possible risk of organism that can be obtained from the given organism is strictly smaller than <span class="tex-span">2<sup class="upper-index">31</sup></span>.</p>

## Output

<p>Output the number of organisms that can be obtained from the base one and which have the total risk of disease occurence not greater than <span class="tex-span"><i>T</i></span>.</p>





```input1
5 3 13
BACAC
4 1 2
1 2 3
2 3 4
3 4 10

```




```output1
5

```



## Note

<p>Explanation: one can obtain the following organisms (risks are stated in brackets): BACAC (11), ACAC (10), BAA (5), B (6), AA (4).</p>
