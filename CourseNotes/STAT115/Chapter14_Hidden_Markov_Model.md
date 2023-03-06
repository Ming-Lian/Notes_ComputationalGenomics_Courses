# 1. Markov Chain
    
![Untitled](pictures/Chapter14_Hidden_Markov_Model_01.png)
    
![Untitled](pictures/Chapter14_Hidden_Markov_Model_02.png)
    
![Untitled](pictures/Chapter14_Hidden_Markov_Model_03.png)
    
![Untitled](pictures/Chapter14_Hidden_Markov_Model_04.png)
    
![Untitled](pictures/Chapter14_Hidden_Markov_Model_05.png)

![Untitled](pictures/Chapter14_Hidden_Markov_Model_06.png)
    
# 2. Hidden Markov Model
    
![Untitled](pictures/Chapter14_Hidden_Markov_Model_07.png)
    
![Untitled](pictures/Chapter14_Hidden_Markov_Model_08.png)

![](pictures/Chapter14_Hidden_Markov_Model_09.png)

# 3. Three problems

## 3.1. Pb(observations): forward, backward procedure
        
Given $\lambda$, how to compute $P(O \mid \lambda)$ observing sequence $O=O_1O_2\cdots O_T$
        
- Burte force method

    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_10.png)
            
    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_11.png)
            
        
    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_12.png)
        
- Dynamic programming: a more effcient approach

  - Forward Procedure
                
    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_13.png)

    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_14.png)
    
    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_15.png)
    
    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_16.png)
    
    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_17.png)

    - Backward Procedure
        
        ![Untitled](pictures/Chapter14_Hidden_Markov_Model_18.png)
        
        ![Untitled](pictures/Chapter14_Hidden_Markov_Model_19.png)
        
        ![Untitled](pictures/Chapter14_Hidden_Markov_Model_20.png)
                
## 3.2. Infer hidden states: forward-backward, Viterbi
        
Given observing sequence $O=O_1O_2\cdots O_T$ and $\lambda$, how to choose state sequence $Q=q_1q_2\cdots q_t$
        
- Solution 1: Forward-Backward Procedure
            
    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_21.png)
    
    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_22.png)

 - Solution 2: Viterbi Algorithm
            
    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_23.png)
    
    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_24.png)
            
    ![Untitled](pictures/Chapter14_Hidden_Markov_Model_25.png)

## 3.3. Estimate parameters: Baum-Welch

How to estimate $\lambda = (A, B, \pi)$ so as to maximize $P(O \mid \lambda)$
        
![Untitled](pictures/Chapter14_Hidden_Markov_Model_26.png)
        
# 4. HMM bioinformatics applications

Gene prediction

![Untitled](pictures/Chapter14_Hidden_Markov_Model_27.png)

Protein structure prediction

![Untitled](pictures/Chapter14_Hidden_Markov_Model_28.png)

Copy number variation

![Untitled](pictures/Chapter14_Hidden_Markov_Model_29.png)

Chromation states/domains prediction

![Untitled](pictures/Chapter14_Hidden_Markov_Model_30.png)

Chromatin topologically associating domains

![Untitled](pictures/Chapter14_Hidden_Markov_Model_31.png)
