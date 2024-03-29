PROJECT TITLE    : Finding a Gene - Using the Simplified Algorithm
AUTHORS          : YUSUF ÇAĞRI DAL
USER INSTRUCTIONS: This assignment is to write the code from the lesson from scratch by following the steps below. This will help you see if you really understood how to put the code together, and might identify a part that you did not fully understand. If you get stuck, then you can go back and watch the coding videos that go with this lesson again. We recommend you try this with many of the future Java coding examples before starting programming exercises.

Specifically, you should do the following:

  1. Create a new Java project named StringsFirstAssignments. You can put all the classes for this programming exercise in this project.

  2. Create a new Java Class named Part1. The following methods go in this class.

  3. Write the method findSimpleGene that has one String parameter dna, representing a string of DNA. This method does the following:

     Finds the index position of the start codon “ATG”. If there is no “ATG”, return the empty string.

     Finds the index position of the first stop codon “TAA” appearing after the “ATG” that was found. If there is no such “TAA”, return the empty string. 
  
    
Print the DNA string. 

See if there is a gene by calling findSimpleGene with this string as the parameter. If a gene exists following our algorithm above, then print the gene, otherwise print the empty string.
