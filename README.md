# MDP REPRESENTATION
```
Date:  ___ / ___ /____
```
## AIM:
To represent a Markov Decision Process(MDP) problem in the following ways.

1. Text representation
2. Graphical representation
3. Python - Dictonary representation

## PROBLEM STATEMENT:

### Problem Description
To develop an environment consisting of a mobile tower as the start and the house as the goal. The aim is to make sure the network signals reaches the house.

### State Space
{0,1,2,3,4,5,6,7}

### Sample State
4

### Action Space
* {0} Moving Up
* {1} Moving Right
* {2} Moving Down
* {3} Moving Left

### Sample Action
{1} Moving Right

### Reward Function
* +1 - If the goal is reached
* 0 - Otherwise

## GRAPHICAL REPRESENTATION:
![MDP DHIV](https://github.com/DhivyaShri484/mdp-representation/assets/94505585/54ce1f51-e3bb-4070-885d-b7ba9834202a)


## PYTHON REPRESENTATION:
```
Developed By : Baggu Dhivya Shri
Reg No.: 212221230009
```
```python
P = {
    0 : {
        0 : [(1.0, 0, 0.0, False)],
        1 : [(1.0, 1, 0.0, False)],
        2 : [(1.0, 2, 0.0, False)],
        3 : [(1.0, 0, 0.0, False)]
    },

    1 : {
        0 : [(1.0, 1, 0.0, False)],
        1 : [(1.0, 1, 0.0, False)],
        2 : [(0.8, 3, 0.0, False), (0.2, 1, 0.0, False)],
        3 : [(0.8, 0, 0.0, False), (0.2, 1, 0.0, False)]
    },

    2 : {
        0 : [(0.8, 0, 0.0, False), (0.2, 2, 0.0, False)],
        1 : [(0.8, 3, 0.0, False), (0.2, 2, 0.0, False)],
        2 : [(1.0, 2, 0.0, False)],
        3 : [(1.0, 2, 0.0, False)]
    },

    3 : {
        0 : [(0.8, 1, 0.0, False), (0.2, 3, 0.0, False)],
        1 : [(1.0, 3, 0.0, False)],
        2 : [(0.8, 4, 0.0, False), (0.2, 3, 0.0, False)],
        3 : [(0.8, 2, 0.0, False), (0.2, 3, 0.0, False)]
    },

    4 : {
        0 : [(0.8, 3, 0.0, False), (0.2, 4, 0.0, False)],
        1 : [(0.8, 5, 0.0, False), (0.2, 4, 0.0, False)],
        2 : [(0.8, 6, 0.0, False), (0.2, 4, 0.0, False)],
        3 : [(1.0, 4, 0.0, False)]
    },

    5 : {
        0 : [(1.0, 5, 0.0, False)],
        1 : [(1.0, 5, 0.0, False)],
        2 : [(0.8, 7, 1.0, True), (0.2, 5, 0.0, False)],
        3 : [(0.8, 4, 0.0, False), (0.2, 5, 0.0, False)]
    },

    6 : {
        0 : [(0.8, 4, 0.0, False), (0.2, 6, 0.0, False)],
        1 : [(0.8, 7, 1.0, True), (0.2, 6, 0.0, False)],
        2 : [(1.0, 6, 0.0, False)],
        3 : [(1.0, 6, 0.0, False)]
    },

    7 : {
        0 : [(1.0, 7, 0.0, True)],
        1 : [(1.0, 7, 0.0, True)],
        2 : [(1.0, 7, 0.0, True)],
        3 : [(1.0, 7, 0.0, True)]
    }
}
```

## OUTPUT:
![image](https://github.com/DhivyaShri484/mdp-representation/assets/94505585/a12cf2cc-abe3-43b5-9462-65c8596bf77e)


## RESULT:
Thus a real world problem is represented as Markov Decision Problem in the following ways successfully: Text Representation, Graphical Representation, Python Representation

