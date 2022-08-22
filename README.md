## Projects informations

### 1 - Sorting algorithms

#### Language: C

#### Description

Implementation of two sorting algorithms, `Quick Sort` and `Binary Insertion Sort`. The code is generic and it accepts different inputs for different sorting options. It comes with unit-test.

#### Usage

The `records.csv` file (omitted) contains 20mln records.
Every record is defined as such:

- id: (integer) unique identifier of the record;
- field1: (string) contains words from the divina commedia, without spaces or commas;
- field2: (integer);
- field3: (floating point);

The format is that of a standard CSV: every field is separated with commas; every record with `\n`.

It also measures the time neeeded to read the file and sort the records.

### 2 - Skip List

#### Language: C

#### Description

The `skip_list` is a probabilistic data structure that allows to perform the search operation (also insertion and deletion) with complexity `O (log n)` in terms of time.

The `skip_list` speeds up the search operation because each node of the `skip_list` contains not only a single pointer to the next element in the list, but an array of pointers that allow us to jump to several subsequent points in the list.

An example of this scheme is shown in the following figure:

![Example of a `skip_list`](skiplist.png)

#### Usage

The file `dictionary.txt` contains words. The words are written in sequence, each on a line.

The file `correctme.txt` contains the text that needs to be corrected. Some words are missing from the dictionary.

### 3 - Heap

#### Language: Java

#### Description

It's a library that realizes the Minimum Heap data structure. The data structure must:
- represent the heap through a vector (it is also possible to use other internal support structures, if necessary);
- allow any number (not known) of elements in the heap;
- be generic in regards of the type of the elements;
- be generic in regards of the criterion of comparison between elements of the heap.

It also needs to offer the following operations:
  - creation of an empty heap - `O(1)`;
  - insert of an element - `O(log n)`;
  - return the heap size - `O(1)`;
  - return the parent of an element - `O(1)`;
  - return the left child of an element - `O(1)`;
  - return the right child of an element - `O(1)`;
  - extraction of the minimum element - `O(log n)`;
  - decreasing the value of an element - `O(log n)`.

### 4 - Dijkstra

#### Language: Java

#### Description

Implementation of a library that builds the `Graph` data structure to be optimal for sparse data.
The structure must allow the representation of both direct and non-direct graphs.

The implementation is generic both in regards to the type of nodes and in regards to the labels of the arches.
It also contains the implementation of Dijkstra's algorithm to determine the shortest paths in a weighted directed graph, having non-negative edge weights.

#### Usage

The application uses the italian\_dist\_graph.csv file (not included) and returns the shortest path from Torino, with both the direct and non-direct graph.

The file contains the distances in meters between locations.
The format is a standard CSV, with fields separated by commas and records separated by `\n`.

Every record contains:
  - locations 1: (string) name of the "source" location.
  - locations 2: (string) name of the "destination" location.
  - distance: (float) distance in meters between the two locations.
