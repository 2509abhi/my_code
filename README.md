# Python code for codechef submission
    
# my_code
# 2509abhi-patch-1
# if_have_better_idea_than_change


//https://www.codechef.com/submit/PALL01

t1=int(input())
for t in range(0,t1):
    N=int(input())
    temp=N
    for i in range(10):
        temp=temp//10
        if(temp==0):
            break
    temp=N
    temp2=0
    i1=i+1
    for j in range((i+1)//2):
        if(temp//(10**(i1-1))==temp%10):
            temp2+=1
        temp%=(10**(i1-1))
        temp=temp//10
        
        if(i1==1):
            break
        i1-=2
    if(temp2==(i+1)//2):
        print("wins")
    else:
        print("loses")

# Talk is cheap show me the code
# main
