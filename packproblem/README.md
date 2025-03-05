# Packing Problem 

## Stage 1

Imagine you're working at a warehouse. You've just received a shipment of products. 

These products are packed in boxes of a certain size: 5, 16, 42, 59. 

For example, a shipment of 52 products could be packed as 4 boxes of 5 and 2 boxes of 16. This combination uses 6 boxes. Or 2 boxes of 5 and 1 boxes of 42. This combination only uses 3 boxes.

We've got a lot of product deliveries to fulfill. Given the list of delivery sizes (your input), find the smallest number of boxes that can be used to pack each delivery. Here's some more simple examples:

Example input: 
```
84
36
90
74
40
```

Answers:
```
2 boxes
84 = (42*2)

5 boxes
36 = (5*4)+(16*1)

4 boxes
90 = (42*1)+(16*3)

3 boxes
74 = (42*1)+(16*2)

8 boxes
40 = (5*8)

Total boxes: 22
```

The full input is [input1.txt](./input1.txt). We want to know the total number of boxes used for all deliveries.

## Stage 2

Great news, we're expanding our business! 

We're now shipping multiple products, each with their own box sizes. They also have different costs.

You'll get two files. One describes the packaging where it first states the packaging type, then lists the box sizes, then it lists the box costs. 

```
A
Size: 5 10 
Cost: 31 19 

B
Size: 9 15 4 
Cost: 53 8 140 
```

The second file is the order list. Each line is an order which starts with the packaging type then the order size. 

```
B 46
A 130
B 76
A 15
B 126 
```

```
5 boxes
46 = (4*1)+(15*1)+(9*3)
Cost: 307 = (140*1)+(8*1)+(53*3)

13 boxes
130 = (10*13)
Cost: 247 = (19*13)

7 boxes
76 = (15*3)+(9*3)+(4*1)
Cost: 323 = (140*1)+(8*3)+(53*3)

2 boxes
15 = (10*1)+(5*1)
Cost: 50 = (19*1)+(31*1)

10 boxes
126 = (15*6)+(9*4)
Cost: 260 = (53*4)+(8*6)

Total boxes: 37
```

Note that some orders can't be fulfilled with the available boxes. You'll need to ignore those. 

You should try and minimise the total cost of the boxes used and should output the number of boxes used for each order. If two orders can be fulfilled with the same cost of boxes, then you should use box combination that uses the fewest boxes.

The order list is [input2.txt](./input2.txt) and the packaging information is [boxdata2.txt](./boxdata2.txt). As before, we want to know the total number of boxes used for all deliveries, ignoring the ones that can't be fulfilled correctly. 
