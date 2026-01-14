# data-cleaning-pipeline-test-on-fuzzy-matching-

Fuzzy Grouping Algorithm  
The core logic of the script is an iterative clustering algorithm that groups titles based on string similarity. The group_titles function iterates through the unique base titles and compares them against existing group keys using rapidfuzz.fuzz.ratio. If a title matches a key with a similarity score of 85 or higher, it is added to that group; otherwise, it establishes a new group key. Finally, the script generates a parent_map dictionary to assign the standardized "Parent Programme" back to the main DataFrame and exports the results to a CSV file.
