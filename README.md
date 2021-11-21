# Patika_Projeler
Patika ödevleri ve proje içerikleri

1. Sorunun cevabı için : 

def duz(veri):
    for deger in veri:
        if isinstance(deger, list):
            yield from duz(deger)
        else:
            yield deger


veri = [[1, 'a', ['cat'], 2], [[[3]], 'dog'], 4, 5]
flatten_v = [penguen for penguen in duz(veri)]

print(flatten_v)
