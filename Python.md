# Proje Sahibi: Patika.Dev 
# Proje Konusu: Veri Yapıları ve Algoritmalar
## Konu : Python

#### 1. Sorunun cevabı için :
- Bir listeyi düzleştiren (flatten) fonksiyon yazın. Elemanları birden çok katmanlı listelerden ([[3],2] gibi) oluşabileceği gibi, non-scalar verilerden de oluşabilir.
```
alpha = []
x=[[1,'a',['cat'],2],[[[3]],'dog'],4,5]
def flatten(x):
    for i in x:
        if type(i) == list:
            flatten(i)
        else:
            alpha.append(i)
    return alpha
flatten(x)
print(alpha)
```

#### 2. Sorunun cevabı için :
- Verilen listenin içindeki elemanları tersine döndüren bir fonksiyon yazın. Eğer listenin içindeki elemanlar da liste içeriyorsa onların elemanlarını da tersine döndürün.
```
y=[[1, 2], [3, 4], [5, 6, 7]]
result=list()
for i in (y[::-1]):
    result.append((i[::-1]))
print(result)
```

