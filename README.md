# -python generator
def Triangle():
    N=[1]
    while True:
          yield N
          N.append(0)
          N=[N[i-1]+N[i] for i in range(len(N))]

n=0
for t in Triangle():
    print(t)
    n=n+1
    if n == 10 :# the value of n can be changed what ever you want.
        break
          

