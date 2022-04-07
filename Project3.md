[Back to Portfolio](./)

Large Map
===============

-   **Class: CSCI 315** 
-   **Grade: In Progress** 
-   **Language(s): C++** 
-   **Source Code Repository:** [features/mastering-markdown](https://guides.github.com/features/mastering-markdown/)  
    (Please [email me](mailto:example@csustudent.net?subject=GitHub%20Access) to request access.)

## Project description

This program is used to find a certain name from a file in an efficient amount of time. It takes input of around 50,000 first and last names and records how long it takes to find them. The Big O notation for search is Log(n) and is fairly efficient.

## How to compile and run the program

Commands and their uses:
plot - compiles the program
data.out - outputs data from file to a file which will need to be renamed
data.pdf - graphs the data from 3 renamed files
mv data.out file.txt - renames data.out to the desired name

```bash
cd ./project1
make plot
make data.out
mv data.out newName.out
```

Note: You will have to change the size in "file-helper2.cpp" to get different sizes to measure the graphs. Find line 12 and change X to a number 50,000 or less.
```bash
const int MAX_NAME_COUNT = X;
```


## UI Design

The user interface is a commandline interface which is directed by user makefile commands. The user will be able to generate a graph using the data on the efficiency of the program.

Lorem ipsum dolor sit amet (see Fig 1), consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat (see Fig 2). Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum (see Fig 3).

![screenshot](images/dummy_thumbnail.jpg)  
Fig 1. The launch screen

![screenshot](images/dummy_thumbnail.jpg)  
Fig 2. Example output after input is processed.

![screenshot](images/dummy_thumbnail.jpg)  
Fig 3. Feedback when an error occurs.

## 3. Additional Considerations

Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. 

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

[Back to Portfolio](./)
