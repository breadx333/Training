Король
```
def printList(lst):
    for i in lst:
        print(i)

m = int(input(":"))
n = int(input(":"))

K = [[0]*m for i in range(n)]

for i in range(n):
    K[i][0] = 1

for j in range(m):
    K[0][j] = 1

for i in range(1, n):
    for j in range(1, m):
        K[i][j] = K[i-1][j-1] + K[i-1][j] + K[i][j-1]

printList(K)
```
Result:
```
[1, 1, 1, 1, 1]
[1, 3, 5, 7, 9]
[1, 5, 13, 25, 41]
[1, 7, 25, 63, 129]
[1, 9, 41, 129, 321]
```
