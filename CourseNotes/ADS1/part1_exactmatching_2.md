# Online vs. offline

![Untitled](pictures/part1_exactmatching_2_01.png)

![Untitled](pictures/part1_exactmatching_2_02.png)

![Untitled](pictures/part1_exactmatching_2_03.png)

# k-mer index

Build k-mer index

![Untitled](pictures/part1_exactmatching_2_04.png)

Query index

![Untitled](pictures/part1_exactmatching_2_05.png)

![Untitled](pictures/part1_exactmatching_2_06.png)

# Data structure

## Ordered structure for indexing

![Untitled](pictures/part1_exactmatching_2_07.png)

![Untitled](pictures/part1_exactmatching_2_08.png)

By using this data structure, we can use binary search for querying index

![Untitled](pictures/part1_exactmatching_2_09.png)

![Untitled](pictures/part1_exactmatching_2_10.png)

![Untitled](pictures/part1_exactmatching_2_11.png)

A useful python module called 'bisect'

![Untitled](pictures/part1_exactmatching_2_12.png)

![Untitled](pictures/part1_exactmatching_2_13.png)
 
## Hash table

![Untitled](pictures/part1_exactmatching_2_14.png)

![Untitled](pictures/part1_exactmatching_2_15.png)

![Untitled](pictures/part1_exactmatching_2_16.png)

![Untitled](pictures/part1_exactmatching_2_17.png)

## Variation on k-mer index

- remove odd offsets

    ![Untitled](pictures/part1_exactmatching_2_18.png)
    
    advantages:
    
    the index now is smaller, take up less memory, it is also a little faster to query
    
    you may wonder if it will cause us to miss some of the matches ?
    
    ![Untitled](pictures/part1_exactmatching_2_19.png)
    
    mostly it would be solved by another indexes
    
    ![Untitled](pictures/part1_exactmatching_2_20.png)

- all the different offsets on multiple 3

    ![Untitled](pictures/part1_exactmatching_2_21.png)

- indexing for subsequences

    ![Untitled](pictures/part1_exactmatching_2_22.png)
    
    ![Untitled](pictures/part1_exactmatching_2_23.png)
    
    ![Untitled](pictures/part1_exactmatching_2_24.png)
    
    advantage: it tends to increase the specificity of the filter provided by the index
