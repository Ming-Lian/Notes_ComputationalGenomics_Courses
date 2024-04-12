![](./pictures/part2_assembly_practice_01.png)

in fact, the graph is big and messy

![](./pictures/part2_assembly_practice_02.png)

why is the graph so messy?

- (1) sequencing errors
    
    sequencing errors can introduce sort of spurious division in the graph, and dead ends
    
    ![](./pictures/part2_assembly_practice_03.png)
    
- (2) redudant edges (specific to overlap graph)
    
    ![](./pictures/part2_assembly_practice_04.png)
    
- (3) polyploidy: can simplify graph by collapsing bobles
    
    ![](./pictures/part2_assembly_practice_05.png)
    
- (4) repeats
    
    ![](./pictures/part2_assembly_practice_06.png)
    
    so basically, we deal with it by chopping the assembly and pieces
    
    so in the end of day, instead of reporting a single assembly genome sequence, an assembler will report a set of contigs
    
    ![](./pictures/part2_assembly_practice_07.png)
    

![](./pictures/part2_assembly_practice_08.png)