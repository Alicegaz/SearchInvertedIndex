# SearchInvertedIndex

Algorithm for building inverted index of the files and then performing a multiword query search 

## To run the programm from the shell

#### in your terminal:

navigate to the path - cd {your path to the project folder}/IdeaProjects/inverted_index1/src/sample
  
run - chmod +x run.sh

and - ./run.sh “{query string}”
  
## Description
In ‘{Your path}/inverted_index1/Dictionary.txt’ direction there is an initial not sorted dictionary of normalized tokens already with duplicates removed
  
In ‘{Your path}/inverted_index1/SortedDictionary.txt’ direction there is the final index (note for readability it was decided not to print out the positions list for each doc entry of the postings list of the term). That index consists of the normalized (punctuation and white spaces removed) and stemmed (Potter’s algorithm was implemented for that purpose ) terms, which are sorted in the alphabetical order. For each term there is the corresponding idf estimate and the postings_list with positions list  and the tf score for each entry.

In the output there is the paths of the documents containing the most relevant results.

