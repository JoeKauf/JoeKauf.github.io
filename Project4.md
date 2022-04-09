[Back to Portfolio](./)

Large Map
===============

-   **Class: CSCI 315** 
-   **Grade: In Progress** 
-   **Language(s): C++** 
-   **Source Code Repository:** [Large Map](https://github.com/JoeKauf/csci-315-spring-2022/tree/master/project3)  
    (Please [email me](mailto:jakaufman@csustudent.net?subject=GitHub%20Access) to request access.)

## Project description

This project visualizes and compares performance differences between two self-Balancing Binary Search Trees. Binary Search Trees are characterized by average case O(log2n) insert, remove, and searching times. However, in certain cases data can be input presorted. This causes the Binary Tree to resemble a linked list eliminating the added benefits of using a Binary Tree. 

	Self-balancing Binary Search Trees seek to mitigate worst case scenario and try to ensure a consistent Log(N) performance. This is achieved by sorting the data when a particular case is reached. This is typically when the height of the tree becomes imbalanced. As we will see, this is not always the case will see with Splay.

## How to compile and run the program

Commands:

plot - compiles the program

data.out - outputs data from individual file to a file which will need to be renamed

mv data.out file.txt - renames data.out to the desired name

data.pdf - graphs the data from 3 renamed files. In order for this to work names must be renamed to "get.out", "mediumGet.out", "largeGet.out"

```bash
cd ./project1
make plot
make data.out
mv data.out newName.out
make data.pdf
```

Note: You will have to change the size in "file-helper2.cpp" to get different sizes to measure the graphs. Find line 12 and change X to a number 50,000 or less. The program must be recompiled three times to be able to plot for the three sizes.
```file-helper2.cpp
12 const int MAX_NAME_COUNT = X;
```


## UI Design

The user interface is a commandline interface which is operated by user makefile commands. The user generates a performance graph based upon the data that has been manipulated.

When the user enters the commands into the terminal (see Fig 1), the program runs behind the scenes. A text file is generated containing the timings for each size (see Fig 2). Once all of the timings have been created and appropriately named, the user can generate a graph (see Fig 3). Fig 4 displays the performance for finding a name's ID for sizes up to 50,000 names.

![screenshot](images/MapCommands.png)  
Fig 1. Command line

![screenshot](images/MapOutData.png)  
Fig 2. Data.out timings

![screenshot](images/PerfHowMany.png)  
Fig 3. Performance graph for finding number of names containing a prefix

![screenshot](images/PerfSearch.png)  
Fig 4. Performance graph for finding a name and its associated ID

## Performance Analysis of Splay

  Splay trees are Binary search trees that keep the most recent elements towards the top of the tree. Every time insertion is called, the new item is placed at the root. Every time an element is looked up it is also placed at the root (Splay Trees). Therefore, more frequently accessed items will be towards the top. This makes it more efficient when items are more frequently accessed or input than others. This also compliments the cache which aids them in being faster than other structures with similar Big O Notation (Locality and Splay Trees). Since memory is slower than caching, if the lookup can be found in the cache it will be faster than an algorithm that looks to memory to access the information (Locality and Splay Trees).

## Performance Analysis of Treap

  Treap is a combination of binary trees and heaps. They take the key and a random priority for each element and organize the tree based off this information. This helps to mitigate the problem of presorted data being input. This randomization prevents the tree from becoming an O(N) traversal when input in ascending order (Definition: Splay Tree). Treaps seek to prevent this and make it more probable that the look up will be Log(N)(Treap). They do this through setting a priority on nodes, replicating randomness for each insertion. This create a greater likelihood that the insertion will be Log(N).

## Splay Tree’s Advantage Over Treap
  Since splay trees place the most recently accessed or added items to the top, the more frequent an item is used, the lookup time should be faster than other trees. They compliment caches which gives them a major advantage over other data structures as cache access is faster than memory access (Locality and Splay Trees, Cornell). Treaps will be fast, but splay should be faster at accessing these elements because they are more frequent and closer to the top than the Treaps more frequent items. As seen in the graph below, Splay is .002 seconds faster than a normal binary search tree and Treap. 

## Treap Tree’s Advantage Over Splaying
  Although Splay Trees are good overall, Treaps have one slight advantage. Splay trees slow down with random searches. Due to Splaying anticipating different frequencies for inputs, it downplays the randomness of inputs. More recently searched items and inputted items will be closer to the top. In order for Treap to find random items it must traverse over previously pushed up items that are unlikely to be generated again. Additionally, with each search comes a rebalancing around the new node. All of these things make Splay slower on random lookups. 
Treap, on the other hand, does not have to worry about these extra operations. Treap generates random data for each node when it is input. Therefore it reflects true randomness better than Splay. It also does not have any extra operations after each search like splay does. Treap is more probable to have Log(N) time with most data inputs and therefore it is a good general data structure to be used on random data (Treap).

## Additional Considerations

  This Project helps in understanding differences between data structures with comparable Big O Notations. Splaying’s biggest advantage comes when data has certain frequencies to it. Treaps are faster regarding randomized data. When standard Binary Search Trees utilize random operations, they are slightly faster in due to not having calculate priority or rebalance as with inputted data. 
  Splaying theoretically should be faster than Treap and Binary Search Trees due to the utilization of caching. This is because memory lookup is slower than caching. When data is organized in a specific way, it complements the cache. This is exhibited in the results from the table below:

## Performance Plots

[Back to Portfolio](./)
