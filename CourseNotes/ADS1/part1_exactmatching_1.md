# naive algorithm

![Untitled](pictures/part1_exactmatching_1_01.png)

![Untitled](pictures/part1_exactmatching_1_02.png)

![Untitled](pictures/part1_exactmatching_1_03.png)

![Untitled](pictures/part1_exactmatching_1_04.png)

![Untitled](pictures/part1_exactmatching_1_05.png)

![Untitled](pictures/part1_exactmatching_1_06.png)

# Boyer-Moore: better naïve algorithm

quit similar with naive algorithm, but it is much clever

![Untitled](pictures/part1_exactmatching_1_07.png)

principle of Boyer-Moore algorithmn

> Learn from character comparisons to skip pointless alignments
>
> Try alignments in left-to-right order, and try character comparisons in right-to-left order
>
> ![Untitled](pictures/part1_exactmatching_1_08.png)

Bad character rule

> Upon mismatch, skip alignments until (a) mismatch becomes a match, or (b) P moves past mismatched character
>
> ![Untitled](pictures/part1_exactmatching_1_09.png)

Good suffix rule

> Let t = substring matched by inner loop; skip until (a) there are no mismatches between P and t or (b) P moves past t
>
> ![Untitled](pictures/part1_exactmatching_1_10.png)

Put 2 rules together

> Use bad character or good suffix rule, whichever skips more
>
> ![Untitled](pictures/part1_exactmatching_1_11.png)

Compare with naive algorithm

![Untitled](pictures/part1_exactmatching_1_12.png)

Preprocess — bulid look-up tables

> Pre-calculate skips. For bad character rule, P = TCGC:
>
> ![Untitled](pictures/part1_exactmatching_1_13.png)
