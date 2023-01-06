# Patika_Sort

# 1.Ödev

[22,27,16,2,18,6] dizisini Insertion Sort algoritması ile çalıştırırsak;  27 ile 22 kıyaslanıp küçükse soluna büyükse sağına yazılır ve dizi sonuna kadar bu şekilde devam edilir. --> 1.Adım: 22,27,16,2,18,6

Dizinin 3.elemanı olan 16, önce 27 ile sonra 22 ile kıyaslanır. Küçük olduğu için sola yazılır.--> 2. Adım [16,22,27,2,18,6] olur.

--> 3. Adım [2,16,22,27,18,6] olur.

--> 4. Adım [2,16,18,22,27,6] olur.

--> 5. Adım [2,6,16,18,22,27] sıralı dizisi elde edilir.


Big O Notation = İşlem sayısı n, n-1, n-2...1 şeklinde olacağından, işlem sayısı toplamı n.(n+1)/2; dominant faktörü n²'dir. O(n²)

18 Sayısı Avarage Case' e girer.

Selection Sort
[7,3,5,8,2,9,4,15,6] dizisini Selection Sort algoritması ile çalıştırdığımızda ilk 4 adımı:

En küçüğü bulup baştaki elemanla yer değiştirerek çalışacaklar.

1.Adım --> [2,3,5,8,7,9,4,15,6]
2.Adım --> [2,3,4,8,7,9,5,15,6]
3.Adım --> [2,3,4,5,7,9,8,15,6]
4.Adım --> [2,3,4,5,6,9,8,15,7]


# 2.Ödev

[16,21,11,8,12,22] -> dizisi Merge Sort ile sıralarken;

Ortadan bölerek ilerleriz.

1.Adım [16,21,11] ,[8,12,22]
2.Adım [16] , [21,11} - [8] , [12,22]
3.Adım [16] , [21] , [11] , [8] , [12] , [22]
4.Adım [16] , [11,21] - [8] , [12,22]
5.Adım [11,16,21] - [8,12,22]
6.Adım [8,11,12,16,21,22]

Big O Notasyonu O(nlogn)

# 3.Ödev

[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]  dizisini Binary Search Tree Aşamaları.

[7,5,1,8,3,6,0,9,4,2] Binary Search Tree'ye göre sıralarken, sıralı diziymiş gibi varsayıp indexte orta noktayı ror alıyor. Bu durumda 10 elemanlı olduğu için 3 veya 6'yı root olarak alabiliriz. Sağ tarafa kendinden büyükler, sol tarafa kendinden küçükler yazılıyor.

             6         0.indexteki 7>6 sağa yazılır. 1.indexteki 5<6 sola yazılır.
            /\
           5  7        2.indexteki 1<6 ve 1<5 sola yazılır. 3.indexteki 8>6 ve 8>7 sağa yazılır.
          /    \
         1      8      4.indexteki 3<6 ve 3>1 sağa yazılır. 6.indexteki 0<6, 0<5, 0<1 sola yazılır.
        /  \     \
       0    3     9    7.indexteki 9>6, 9>7, 9>8 sağa yazılır.
            /\
           2  4        8.indexteki 4<6, 4<5, 4>1, 4>3 sağa yazılır. 
           
                       9.indexteki 2<6, 2<5, 2>1, 2<3 sola yazılır.