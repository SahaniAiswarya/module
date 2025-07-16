rows=int(input("enter rows"))
pattern=[''.join(['*' for j in range(i)]) for i in range(1,rows+1)]
for line in pattern:
        print(line)


rows=int(input("enter rows"))
pattern=[''.join([chr(97+j) for j in range(i)]) for i in range(1,rows+1)]
for line in pattern:
        print(line)


rows=int(input("enter rows"))
pattern=[''.join([str(num) for num in range(1,rows-i+1)]) for i in range(rows)]
for line in pattern:
        print(line)


n=int(input("enter rows"))
pattern=[['*' if i==0 or i==n-1 or j==0 or j==n-1 else ' ' for i in range(n)] for j in range(n)]
for i in pattern:
        print(''.join(i))


n=int(input("enter rows"))
upper=[' '*(n-i)+''.join('*' if j==0 or j==2*i else ' ' for j in range(2*i+1)) for i in range(n)]
lower=[' '*(i+2)+''.join('*' if j==0 or j==2*(n-i-2) else ' ' for j in range(2*(n-i)-1)) for i in range(n-1)]
for line in upper+lower:
        print(line)

        
