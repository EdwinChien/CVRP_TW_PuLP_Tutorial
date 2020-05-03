# **Hellow World!!**
## © Chun Lin, Chien (2020)
## **Note 1. This tutorial is written by Chun Lin, Chien on 2020-05-02 with python PuLP linear programming module for Vehicle Routing Problem with Capacity limitation and Time window.**
---
```
P.S : If you use this CVRP_TW python code or refer the result in your research, please cite this tutorial.
      ( e.g, python PuLP tutorial for CVRP_TW (Chien, 2020) ).
```
---

## Note 2. Before you use this code, their are few things you must know...
```
Hint 1: This code is written in Google Colaboratory environment, if you want to run it directly, please copy the files to your google drive and work with Google Colaboratory.

Hint 2: Each time you use PuLP in a Google Colaboratory ipython notebook, make sure you have installes PuLP in your working environment.

Hint 3: This code only contains the multi-vehicle version (i.e., dynamic capacity version), if you are interested in the static capacity version, please contact me.
```
## Appendix: Solved results and duration list.
### Config 1. Static vehicle capacity (default value = 18).
```
CVRP ( Max capacity = 18 )

Duration = 427 ms

Shortest distance = 10987.0

Vehicle — 0 : Chicago (0) -> Hous (7) -> KC (7) -> Chicago (0) →→→ Total demand = 14 units.

Vehicle — 1 : Chicago (0) -> LA (18) -> Chicago (0) →→→ Total demand = 18 units.

Vehicle — 2 : Chicago (0) -> Oakl (4) -> Frsn (3) -> Anah (5) -> Den (6) -> Chicago (0) →→→ Total demand = 18 units.
```
### Config 2. Dynamic vehicle capacity.
```
CVRP ( Multi-Vehicle capacity )

# capacity = [14, 18, 18, 24, 36]

Duration = 15.5 s

Shortest distance = 10483.0

● Vehicle — 0 (Total capacity=14) : Chicago (0) -> Hous (7) -> KC (7) -> Chicago (0) →→→ Total demand = 14 units.

● Vehicle — 1 (Total capacity=18) : Chicago (0) -> Oakl (4) -> Frsn (3) -> Anah (5) -> Den (6) -> Chicago (0) →→→ Total demand = 18 units.

● Vehicle — 2 (Total capacity=18) : Chicago (0) -> LA (14) -> LA_2 (4) -> Chicago (0) →→→ Total demand = 18 units.
```
### Config 3. Dynamic vehicle capacity with Time window.
```
CVRP_TW ( Multi-Vehicle capacity )

# capacity = [14, 18, 18, 24, 36]

Duration = 2.62 s

Shortest distance = 10483.0

● Vehicle — 0 (Total capacity=14) : Chicago (0) -> Hous (7) -> KC (7) -> Chicago (0) →→→ Total demand = 14 units.

● Vehicle — 1 (Total capacity=18) : Chicago (0) -> Den (6) -> Anah (5) -> Frsn (3) -> Oakl (4) -> Chicago (0) →→→ Total demand = 18 units.

● Vehicle — 2 (Total capacity=18) : Chicago (0) -> LA_2 (4) -> LA (14) -> Chicago (0) →→→ Total demand = 18 units.
```
---
### Solution Visualization : Final solution route map.
![CVRP_TW](https://github.com/EdwinChien/CVRP_TW_PuLP_Tutorial/blob/master/CVRP_TW_route.png)

---
