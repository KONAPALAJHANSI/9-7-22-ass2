class sol(object):
    def count(self,n):
        count=0
        prime=[False for i in range(n+1)]
        for i in range(2,n):
            if prime[i]==False:
                count+=1 
                j=2
                while j*i<n:
                    prime[j*i]=True
                    j+=1 
        return count
ob1=sol()
print(ob1.count(50))
