# arangodb
Notes from arangodb course

Run arangodb via terminal: `arangosh`

3.16 <br>
Simple query from section-3/filter.aql takes 597,228 ms (hundreds, not thousands). Number of times query had to iterate through the flights collection is 286463 (total number of edges in the flights collection) to return only 97 results. This is inefficient and can be improved by creating an index.

![Alt text](image.png)

After creating above index the same query runs in 1,250 ms.

**Conclusion**: Indexes fix the problem of slow running queries.