
# Insertion Sort algoritması şu şekildedir:

Dizinin ilk elemanını seçin ve onu sıralanmış kabul edin.
Dizinin diğer elemanlarını sıralanmış bölümdeki uygun yerlerine ekleyin, uygun yer bulmak için sıralanmış bölümdeki elemanlarla karşılaştırın ve konumunu belirleyin.
Dizi tükenene kadar 2. adıma devam edin.</br></br>

## [22,27,16,2,18,6] dizisinin Insertion Sort'a göre aşamaları şöyle olur:

- [22] [27,16,2,18,6]
- [22,27] [16,2,18,6]
- [16,22,27] [2,18,6]
- [2,16,22,27] [18,6]
- [2,16,18,22,27] [6]
- [2,6,16,18,22,27]</br></br>

### Big-O gösterimi: Insertion Sort, O(n^2) zamana sahip bir algoritmadır. En iyi durumda (dizi zaten sıralı ise) zaman karmaşıklığı O(n) olabilir.

### Time Complexity: Dizi sıralandıktan sonra 18 sayısı, Average case'e girer. Çünkü 18 sayısı, aranacak sayının ortada olduğu bir durumdur.</br></br>

## [7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımı şöyle olur:

+ [2,3,5,8,7,9,4,15,6]
+ [2,3,4,8,7,9,5,15,6]
+ [2,3,4,5,7,9,8,15,6]
+ [2,3,4,5,6,9,8,15,7]</br>
</br>Selection Sort algoritması şu şekildedir:

Dizinin ilk elemanını en küçük eleman olarak seçin.
Dizinin geri kalan elemanlarını bu elemanla karşılaştırın ve daha küçük olanı seçin.
Seçilen elemanı sıralanmış kabul edin ve kalan elemanlar için 2. adıma geri dönün.
Dizi tükenene kadar 2-3 adımlarını tekrarlayın.
Algoritma Kodu:

```
def selection_sort(arr):
    n = len(arr)
    for i in range(n):
        min_idx = i
        for j in range(i+1, n):
            if arr[j] < arr[min_idx]:
                min_idx = j
        arr[i], arr[min_idx] = arr[min_idx], arr[i]
    return arr
```
</br></br>

# Merge Sort'a göre aşamaları şu şekildedir:

- [16,21,11] [8,12,22]
- [16,21] [11] [8,12] [22]
- [16] [21] [11] [8] [12] [22]
- [16,21] [8,11] [12,22]
- [8,11,16,21] [12,22]
- [8,11,12,16,21,22] </br></br>
Big-O gösterimi: Merge Sort, O(n log n) zamana sahip bir algoritmadır.</br></br>

 # Binary-Search-Tree: 

```
       7
     /   \
    5     8
   / \     \
  1   6     9
   \       /
    3     0
     \
      4
       \
        2
        
```

</br>
BST aşamaları şu şekildedir:

- 7 kök düğüm olarak seçilir.
- 5, 1 ve 8 sırasıyla 7'nin sol alt ağacına, sol çocuğu ve sağ alt ağacına eklenir.
- 3, 6, 9 sırasıyla 5'in sağ alt ağacına, sol çocuğuna ve 8'in sağ alt ağacına eklenir.
- 0, 4 ve 2 sırasıyla 3'ün sağ çocuğuna, 4'ün sağ çocuğuna ve 2'nin sağ çocuğuna eklenir.
<p>Bu şekilde BST, verilen dizi elemanlarını sıralı bir şekilde tutar.</p>
</br></br>

---

![Proje](https://kodluyoruz.org/wp-content/uploads/2022/05/kodluyoruz_yatay_slogan-300x35.png)


Bu repo [Kodluyoruz](https://www.kodluyoruz.org/) Algoritma ödev Reposu. İçerisinde bir adet README dosyası barındırıyor.

## Installation

Öncelikle projeyi clonelayın.

```
https://github.com/mucahidcanbey/algoritma_odev.git
```

## Usage

Projeyi cloneladıktan sonra Visual Studio Code programında açınız.

Linux için:

```
cd algoritma_odev
code .
```

## Contributing
Pull requestler kabul edilir. Büyük değişiklikler için, lütfen önce neyi değiştirmek istediğinizi tartışmak için bir konu açınız.

## License
[MIT](https://choosealicense.com/licenses/mit/)