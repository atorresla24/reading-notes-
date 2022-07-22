# Reading Class 05

## Linked List

Node 1, Value: 4 (Head/Current)
                \
                /
Node 2, Value: 8
                \
                /
Node 3, Value: 15
                \
                /
Node 4, Value: 16
                \
                /
Node 5, Value: null

- Node 1 is the head and current node and it is just a starting point to begin traversing through the different nodes

Node 1, Value: 4 (Head)
                \
                /
Node 2, Value: 8 (Current)
                \
                /
Node 3, Value: 15
                \
                /
Node 4, Value: 16
                \
                /
Node 5, Value: null

- A *while* loop is used to go through the different nodes until we hit a node that has a value of **null**

Node 1, Value: 4 (Head)
                \
                /
Node 2, Value: 8 
                \
                /
Node 3, Value: 15
                \
                /
Node 4, Value: 16
                \
                /
Node 5, Value: null (Current/end)

- The program will continue to go to the next node until it hits a value of null and then it will end

- In this specific example the Big O of time would be O(5) and Big O of time is O(1)

- A new node can also be added to an already existing node chain through the method Add

New Node, Value 1
                  \
                  /
Node 1, Value: 4 (Head)
                \
                /
Node 2, Value: 8 
                \
                /
Node 3, Value: 15
                \
                /
Node 4, Value: 16
                \
                /
Node 5, Value: null (Current/end)

- The next step to be taken would be to reassign the Head of the node to intake the new node if it is placed before the original Head node

New Node, Value 1 (Head)
                \
                /
Node 1, Value: 4
                \
                /
Node 2, Value: 8 
                \
                /
Node 3, Value: 15
                \
                /
Node 4, Value: 16
                \
                /
Node 5, Value: null (Current/end)

