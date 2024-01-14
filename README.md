## The Jeffrey Epstein Documents — Named Entity Search

By: Shirsho Dasgupta (2023)

The code reads the unsealed and unredacted court records (released January, 2024) and uses a named entity recognition model (spaCy) to sift through them and highlight names by entity-types. This enabled Miami Herald reporters to refer to a makeshift index of names and report out stories quickly. 

The final spreadsheet can be found [here](https://github.com/shirshod/epstein_records/tree/main/epstein_index.csv).

#### Note: 
1. This example uses only a fraction (~60) of all of the unsealed court records that were released.
2. Each of the models (large, medium and small) had minor discrepancies in identifying names. To capture the most number, the code runs all three models, combines them and then deletes duplicates if they are from the same file. 
3. The models classified some people as "ORG" and some organizations as "PERSON".
