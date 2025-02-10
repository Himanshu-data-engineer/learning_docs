# Learning Docs

This repo is for learning via Documents


```
print("=================Given a list============")
lis=[1,2,3,4,5]
print(lis)

print("=============converted given list to rdd================")
rddin=sc.parallelize(lis)
print(rddin.collect())

print("=================multiply with 5 in the rdd list===========")
mulrdd=rddin.map(lambda x : x*5)
print(mulrdd.collect())

print("===============filtered data==============")
fildata=rddin.filter(lambda x : x>2)
print(fildata.collect())
```