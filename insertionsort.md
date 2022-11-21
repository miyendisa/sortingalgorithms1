>**1) [22,27,16,2,18,6] dizinin insertion sort türüne göre aşamalarını yazınız.**
* Öncelikle dizinin ilk elemanı olan 22'yi ele alalım. 22'nin kısmen sıralanmış dizide olduğunu düşünüyoruz.
    
     * [22,27,16,2,18,6]
 

* Dizinin ikinci elemanı olan 27'yi ele alalım. 27 > 22 olduğundan 22 ve 27 kısmen sıralanmış dizidedir.
    
     * [22,27,16,2,18,6]

* Dizinin üçüncü elemanı olan 16'yı ele alalım. 16 < 22 olduğundan  doğru konuma yerleştirelim. Artık 16,22 ve 27 kısmen sıralanmış dizidedir.
    
     * [16,22,27,2,18,6]
* Dizinin dördüncü elemanı olan 2'yi ele alalım. 2 < 16 olduğundan doğru konuma yerleştirelim. Artık 2, 16, 22 ve 27 kısmen sıralanmış dizidedir.
    
  * [2,16,22,27,18,6]
 * Dizinin beşinci elemanı olan 18'i ele alalım. 16'dan büyük ancak 22'den küçük olduğu için doğru konuma yerleştirelim. Artık 2, 16, 18, 22 ve 27 kısmen sıralanmış dizidedir.
    
   * [2,16,18,22,27,6]
  * Dizinin son elemanı olan 6'yı ele alalım. 2'den büyük ancak 16'dan küçük olduğu için doğru konuma yerleştirelim. Artık 2, 6, 16, 18,22 ve 27 sıralanmış şekildedir.
    
    * [2,6,16,18,22,27]

---

>**2) Verilen dizinin Big-O gösterimini yapınız.**

Yazılan bir algoritmanın performansının iyi olması gerekmektedir. Algoritmanın performansını veya Time Complexity'sini hesaplamak için Big-O Notation kullanılır. 
* Insertion Sort sıralaması yaparken dizinin ilk elemanının kısmen sıralanmış dizide olduğunu düşündük.
* Insertion Sort algoritması n elemanlı bir listenin ikinci elemanı için en fazla 1 karşılaştırma ve 1 yer değiştirme yapar. Dolayısıyla verilen dizinin ikinci elemanı olan 27 sayısı için en fazla 1 karşılaştırma ve 1 yer değişikliği söz konusu olabilir.
* Bu sıralama algoritması dizinin üçüncü elemanı için en fazla 2 karşılaştırma ve 2 yer değişikliği, dördüncü eleman için ise en fazla 3 karşılaştırma ve 3 yer değişikliği yaparak devam edecektir. Son eleman için en fazla (n-1) karşılaştırma ve (n-1) yer değişikliği yapacaktır.
* Elimizdeki dizinin elemanları için yapılacak en fazla karşılaştırmalar ve yer değişiklikleri hesaplandığında sonuç;  
n(n-1) = n²-1 olur.

Dolayısıyla Big-O Notation = O(n²) 

---

>**3) Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız**

>* **Average case:** Aradığımız sayının ortada olması
> * **Worst case:** Aradığımız sayının sonda olması
> * **Best case:** Aradığımız sayının dizinin en başında olması

**Dizinin sıralı hali:**  [2,6,16,18,22,27].             
Aradığımız 18 sayısı dizinin ortasında bulunduğundan dolayı average case kapsamındadır.