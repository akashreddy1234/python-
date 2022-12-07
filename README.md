# python-
converting roman to integers
while(1):
    s=input("Enter input:")
    d={"I":1,"V":5,"x":10,"C":100,"D":500,"M":1000}
    sum=0
    n=len(s)
    for i,c in enumerate(s):
        if(i<n-1 and d[c]<d[s[i+1]]):
            sum-=d[c]
        else:
            sum+=d[c]
    print("Corresponding integer of",s,"is:",sum)
