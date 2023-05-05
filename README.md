Download Link: https://assignmentchef.com/product/solved-csf211-assignment2
<br>
<h1>A: Ghot’s Riddle</h1>

The students taking the C programming course recently learnt how to find the <em>n<sup>th </sup></em>number in the fibonacci sequence, but found it to be too easy. So they asked the class ghot to come up with a more difficult function to find. The relation he came up with is defined as follows:

)       if <em>x </em>has two or more distinct divisors other than 1 and itself

(<em>x</em>) =

<em>x                                      </em>if <em>x </em>has 1 divisor or less apart from 1 and itself

Where <em>div</em><sub>1 </sub>and <em>div</em><sub>2 </sub>are the two largest distinct divisors of <em>n</em>, other than 1 and the number itself. In this question, you will be provided with a number <em>n </em>and your task is to find <em>f</em>(<em>n</em>). <em>Note: this is </em><em>not the Fibonacci sequence defined above. Please read the question.</em>

<strong>Input</strong>

The first line of input contains a single integer <em>N </em>(1 ≤ <em>N </em>≤ 10<sup>5</sup>), for which you must find <em>f</em>(<em>N</em>).

<h2>Output</h2>

The output should contain a single integer that is the answer as described by the function above.

input 10

output 7

explanation <em>f</em>(10) = <em>f</em>(5)+<em>f</em>(2), Since 5 and 2 do not have any proper divisors, <em>f</em>(5) = 5 and <em>f</em>(2) = 2 and hence <em>f</em>(10) = 5 + 2 which is equal to 7.

input 8

output

6

<h1>B: Tourism</h1>

One day you decide to visit the Grand Line for some sightseeing. The grand line consists of <em>N </em>different islands numbered from 1 to <em>N</em>. The waters between the Grand Line are incredibly dangerous and it’s easy to get lost, so you buy a log pose to help you navigate. Depending on the island you are currently standing on, the log pose points to zero or more other islands and you can travel to any of these islands. You can start your journey from any island initially. You want to know the maximum number of <strong>distinct </strong>islands that can be reached from a starting island of your choice (the island you start from should also be counted) <em>Note that from your current island you can only travel to an island that the log pose points to</em>. <em>Keep in mind that you need to find the maximum number of islands that you can possibly reach from the starting island, not a path with the largest number of islands. See sample case for clarity.</em>

<h2>Input</h2>

The first line of input contains two space-separated integers <em>N </em>and <em>M </em>(1 ≤ <em>N </em>≤ 1000, 0 ≤ <em>M </em>≤ 1000) denoting the number of islands and island transitions you can make respectively. In the <em>M </em>lines that follow, the <em>i<sup>th </sup></em>line containing two space-separated integers, <em>U<sub>i </sub></em>and <em>V<sub>i </sub></em>representing that from island <em>U<sub>i</sub></em>, one of the islands that the log pose points to is <em>V<sub>i</sub></em>.

<h2>Output</h2>

Print a single integer X denoting the maximum number of islands that you can reach if you start from some island.

input

5 5

1 2

1 5

5 4

5 3

3 2

output 5

explanation

if we draw the corresponding possible paths between islands, we can see that from the island 1 we can reach all other islands. From 2, we can’t reach any other node. from 3 we can reach 3 and 2. from 4 we can reach only itself. from 5 we can only reach

5 and 4. Clearly we can see that if we start from node 1 our answer would be 5 which is maximum possible.

<h1>C: Klutz</h1>

<em>N </em>people are participating in the binary blitz competition this time, each numbered from 1 to <em>N </em>and all of them have a particular rating on codeforces. It is known that if two people compete, the one with the higher rating wins for sure. It is guaranteed that the ratings of all the <em>N </em>people are unique. The problem is that no one provided their actual codeforces handle so you don’t know anyone’s rating. All the <em>N </em>people play exactly once against every other person. So obviously there will be a total of games in total played by the <em>N </em>people. The competition is over and you have kept a record of all the matches in the following format: You have rows, and each row containing two space separated integers. The first number of these is the winner and the second one is the loser. It turns out you have lost exactly one row from this list and you have to try and fill in the missing record so that it doesn’t contradict any of the other rows. If it is not possible to determine the winner and loser, print them in any order.

<h2>Input</h2>

The first line contains a single integer <em>N </em>which is the number of people participating (3 ≤ <em>N </em>≤ 200).

The following 1 lines contain two space-separated integers each <em>U<sub>i </sub></em>and <em>V<sub>i</sub></em>, where <em>U<sub>i </sub></em>is the winner of that round and <em>V<sub>i </sub></em>is the loser.<em>As an extra challenge, try to solve this with the constraint</em>

3 ≤ <em>N </em>≤ 2000<em>.</em>

<h2>Output</h2>

Output a single line containing two space-separated integers that is the missing entry. If you cannot determine the winner and loser with the give information then print them in any order

input

4

4 2

4 1

<ul>

 <li>1</li>

 <li>1</li>

</ul>

2 3

output

4 3

explanation

notice that if we put 3 4 then it would contradict line 1 and line 5

<h1>D: Geass Code</h1>

You are the leader of the resistance against Britannia and you have <em>N </em>Knightmares that you can use during the revolution. The <em>i<sup>th </sup></em>Knightmare initially has a power <em>P<sub>i</sub></em>. You decide that the current power of your Knightmares isn’t enough so you ask your lead scientist Rakshata to help you out. She comes up with <em>M </em>power multipliers placed one after the other in a row. each multiplier has a different power where <em>i<sup>th </sup></em>multiplier has a power <em>Mult<sub>i</sub></em>. She uses this in the following way: Start by placing the first index of the multiplier over the first element in <em>P</em>. Then for all 1 ≤ <em>i </em>≤ <em>M</em>, <em>P<sub>i </sub></em>= <em>P<sub>i </sub></em>· <em>Mult<sub>i</sub></em>. Then move the starting position of the multiplier to the second position of <em>P</em>. Then for all 1 ≤ <em>i </em>≤ <em>M</em>, <em>P<sub>i</sub></em><sub>+1 </sub>= <em>P<sub>i</sub></em><sub>+1</sub>·<em>Mult<sub>i</sub></em>. Then move the starting position of the multiplier over to the third element of <em>P </em>and for all <em>i </em>1 ≤ <em>i </em>≤ <em>M</em>, <em>P<sub>i</sub></em><sub>+2 </sub>= <em>P<sub>i</sub></em><sub>+2 </sub>· <em>Mult<sub>i</sub></em>. Keep moving the starting position of the multiplier and multiplying its elements in a similar manner. Do this process a total of <em>n</em>−<em>m</em>+1 times. You must output the final powers of all the knightmares after all the operations are completed. Since the numbers can be very large, output them modulo (10<sup>9 </sup>+ 7). <em>Note: Please ensure to use long int/long long int to avoid integer overflow since upon multiplication, the numbers can exceed the size of int.</em>

<h2>Input</h2>

The first line consists of two space-separated integers <em>N </em>and <em>M</em>, the number of Knightmares and the number of multipliers. (1 ≤ <em>M </em>≤ <em>N </em>≤ 10<sup>5</sup>). The second line contains <em>N </em>space-separated integers which are the initial powers of the knightmares <em>P</em><sub>1</sub><em>,P</em><sub>2</sub><em>,…,P<sub>n</sub></em>. The third line contains <em>M </em>space-separated integers, representing the power of each of the <em>M </em>multipliers, <em>A</em><sub>1</sub><em>,A</em><sub>2</sub><em>,…,A<sub>m </sub></em>(1 ≤ <em>P<sub>i</sub>,A<sub>i </sub></em>≤ 10<sup>9 </sup>∀<em>i</em>).

<h2>Output</h2>

Print a single line of <em>N </em>space-separated integers, the final powers of the knightmares after all operations modulo (10<sup>9 </sup>+ 7).

input

5 3

5 3 1 7 2 1 2 4

output

5 6 8 56 8

explanation

Initially the array <em>A </em>gets multiplied on to the first three elements of <em>P</em>, then the second three, and so on. It is easy to see that this is the answer.

<strong>E: Who Will Win Today?</strong>

Shirogane wants to impress Kaguya and so he tells her that given a set of letters from the english alphabet, he can enumerate all possible words of length K using only those letters in 1 second or less. Obviously, this is an impossible task so he asks you, Ishigami, to bail him out so that he doesn’t look stupid in front of Kaguya.

<h2>Input</h2>

The first line consists of two space-separated integers <em>N </em>and <em>K</em>, the number of letters you can use, and the length of each word respectively (it is guaranteed that <em>N<sup>K </sup></em>≤ 10<sup>5 </sup>and sum of lengths of all possible words does not exceed 10<sup>5</sup>). The second line contains a string of <em>N </em><strong>distinct </strong>lowercase English alphabets (no capital letters or special characters) representing the possible letters that you can use. Note that you cannot use any character or letter not present in the string.

<h2>Output</h2>

print <em>N<sup>K </sup></em>lines, each line containing a distinct string of length <em>K</em>. Two strings are considered distinct if they differ in at least one position.

input

2 3

ab

output aab bbb abb bab baa aba bba aaa

<h1>F: Koro-sensei and the Powers of Two</h1>

While the students of class 3E thought they bought some respite after last week’s problem on primes, Koro-sensei is back at it again, with another weird question. Given a number <em>N</em>, the students have to find the <em>number of ways </em>it can be represented as a sum of power of 2. Can you help them?

<strong>Input</strong>

The only line of input contains a single integer N. (0 ≤ N ≤ 10<sup>2</sup>)

<h2>Output</h2>

Print one integer, <em>X </em>denoting the number of ways <em>N </em>can be expressed as a sum of powers. Please note that reorderings of the same sum do not count as multiple ways – eg. (2+2+1), (2+1+2), (1+2+2) are all treated as the same thing.

input 7

output 6

explanation

7 can be represented as: (4 + 2 + 1), (4 + 1 + 1 + 1), (2 + 2 + 2 + 1), (2 + 2 + 1 + 1 + 1), (2+1+1+1+1+1), and (1+1+1+1+1+1+1), since the powers of 2 are 2<sup>0</sup><em>,</em>2<sup>1</sup><em>,</em>2<sup>2 </sup><em>… </em>which are 1<em>,</em>2<em>,</em>4<em>…</em>

input 4

output 4

explanation

(4)<em>,</em>(2 + 2)<em>,</em>(2 + 1 + 1)<em>,</em>(1 + 1 + 1 + 1)

<h1>G: The COVID Vaccine</h1>

It’s finally here and all this can end! However, before normalcy can completely return, enough people need to be vaccinated for everything to be safe. The owner of a vaccine manufacturing facility wants to start selling and shipping vaccines as soon as possible. However, business being business, she wants to ensure that the company spends the <em>least </em>amount of money for shipping the products. Vaccines are first stored in small boxes, which are then stacked inside big boxes before being loaded onto cargo ships and planes. All big boxes have a fixed weight <em>B</em>, but the weights of the small boxes can vary considerably. Given a list of weights of <em>N </em>small boxes, what is the <em>minimum </em>number of big boxes you’d need to ship all the vaccines available? <strong>At most two boxes </strong>(<em>s<sub>i</sub>,s<sub>j</sub></em>) <strong>can be placed in one big box</strong>, due to government regulations. <em>s<sub>i </sub></em>+ <em>s<sub>j </sub></em>≤ <em>B</em>. <em>Additional thinking: How would the answer change if this government regulation was removed? To be clear this is </em><em>not a part of the problem statement – just something to think about.</em>

<h2>Input</h2>

The first line of input contains <em>N </em>(1 ≤ <em>N </em>≤ 2×10<sup>3</sup>). The second line of input contains a sequence of <em>N </em>space-separated integers (<em>s<sub>i </sub></em>≤ <em>B </em>≤ 10<sup>4</sup>), representing the weights of the small boxes that we have. The third line of input contains the number <em>B</em>, the weight of the large box.

<h2>Output</h2>

Print a single integer X denoting the minimum number of large boxes you would need.

input                                                                                         input

2                                                                                                10

<ul>

 <li>1 9 12 7 5 4 3 3 1 8 4</li>

 <li>13</li>

</ul>

output                                                                                      output

1                                                                                                5

explanation                                                                             explanation

We can fit both these small boxes in                                   One valid configuration: (12, 1),

one big box of size 3                                                                    (9, 4), (8, 5), (7, 4), (3,3)

<h1>H: Aggregating the Binary Tree</h1>

You are given a complete binary tree in which all the nodes are at the same depth relative to the root. The binary tree is represented as an array <em>A</em>, where <em>A</em>[0] is the root. For every <em>i<sup>th </sup></em>index, it’s left child is stored in <em>A</em>[2<em>i </em>+ 1] and its right child in <em>A</em>[2<em>i </em>+ 2]. You need to aggregate all the elements in the binary tree following a special rule: <em>S </em>= <sup>P</sup><em><sub>i </sub>A<sub>i </sub></em>× <em>L<sub>i</sub></em>, where <em>A<sub>i </sub></em>is the value at that node and <em>L<sub>i </sub></em>is the level. <em>Note: the level of the root node is 1, and the level of it’s children would be 2, it’s grandchildren 3, and so on.</em>

<h2>Input</h2>

The first line contains a single integer N (1 ≤ <em>N </em>≤ 2<sup>18 </sup>−1) denoting the number of elements in the binary tree where <em>N </em>is of the form 2<em><sup>k </sup></em>− 1 where <em>k </em>is a positive integer. The next line contains N positive space separated integers.

<h2>Output</h2>

Print a single integer S, denoting the aggregate sum of the binary tree.

input 3

21 9 7

output 53

explanation

The root of the binary tree is 21 (level 1), while it’s left child is 9 (level 2) and its right child is 7 (level 2). Aggregated sum = (21 × 1) + (9 × 2) + (7 × 2) = 53

input 7

1 2 4 6 7 5 3

output 76

explanation

1 ∗ 1 + (2 + 4) ∗ 2 + (6 + 7 + 5 + 3) ∗ 3 = 76

<h1>I: The Dinosaur Conundrum</h1>

The inauguration of the Jurassic Park is about to happen tomorrow, and John Hammond has a problem on his hands. While they could successfully clone <em>N </em>different species of dinosaurs, they soon realized that dinosaurs would start attacking each other as soon as they woke up. After a lot of observation, the handlers notice that not all dinosaurs are aggressive towards each other only dinosaurs that have been cloned from the same raw genetic material fight each other. Each dinosaur has a tag, which indicates the source of their genetic material. If the tags of two dinosaurs start with the same first character, they fight, otherwise they don’t. You have <em>C </em>different cages to store the dinosaurs in, each of which can store any number of dinosaurs. Given the tags of all <em>N </em>dinosaurs, separate the dinosaurs into cages such that a <em>minimum </em>number of pairs of dinosaurs fight. For eg, if a cage has three dinosaurs – (“XAHSG-2737”, “XAGFS-89” and “XSGFS-999”) each dinosaur will fight with the other two to form 3 pairs of fights – (“XAHSG-2737”, “XAGFS89”), (“XAHSG-2737”, “XSGFS-999”), (“XAGFS-89” and ”XSGFS-999”).

<h2>Input</h2>

The first line of input contains two space-separated integers, <em>N </em>and <em>C</em>. The following <em>N </em>lines contain strings (of length ≤ 20) denoting the tags of all the dinosaurs. It is guaranteed that the characters in the tag will be from the set [A-Z,0-9].

<h2>Output</h2>

Print one integer, <em>P</em>, the number of pairs of fights that will happen in the minimal case.

<table width="336">

 <tbody>

  <tr>

   <td width="97">input6 4XGB189ABFG99XFG983BST535TIN846 XC67TPoutput0</td>

   <td width="239">input6 2FFT998DFFT99BWFT36BERT99BLIP87 BHIJ78output2</td>

  </tr>

 </tbody>

</table>

<h1>J. Air Tickets</h1>

You have been invited to the Annual Computing Conference which is going to be held in Tokyo this year. Sadly, the organizers have declined to reimburse your flight tickets to the conference. So, you decide to take the flight path (a flight path may have multiple hops) to Tokyo which will cost you the least. Given the all the hops possible between the major cities of the world, find the cost of the minimum flight path. Assume that each hop costs you the same, i.e. $100. <em>Note: You must use adjacency lists to solve this problem.</em>

<h2>Input</h2>

The first line of input contains four space-separated integers N (1 ≤ N ≤ 5000), M (0 ≤ M ≤

N-1) and T (0 ≤ T ≤ N-1) denoting the number of cities, the number of hops,

the city you live in and city you wish to reach (Tokyo) respectively. The following M lines contain two space-separated integers <em>U<sub>i </sub></em>and <em>V<sub>i </sub></em>(0 ≤ <em>U<sub>i</sub></em>, <em>V<sub>i </sub></em>≤ N-1) denoting an undirected hop between the cities <em>U<sub>i </sub></em>and <em>V<sub>i</sub></em>. It is guaranteed that atleast one flight path exists to Tokyo.