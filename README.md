# patikaa
patikaa

1- Bir listeyi düzleştiren fonksiyon yazın.

li=[]
def flatten(n):
     for i in n:
         if isinstance(i,list):#Kontrol ediyor liste mi diye
          flatten(i)
         else:
          li.append(i)#Eğer liste değilse boş olan li elemanına ekliyor


liste=[[1,'a',['cat'],2],[[[3]],'dog'],4,5]
flatten(liste)
print(li)

2- Verilen listenin içindeki elemanları tersine döndüren bir fonksiyon yazın. 


def reverse_list(n):
 n = n[::-1]
 n = [i[::-1] for i in n]
 return n

liste1=[[1, 2], [3, 4], [5, 6, 7]]


print(reverse_list(liste1))
