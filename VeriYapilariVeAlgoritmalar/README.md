# Insertion Sort

[22,27,16,2,18,6] => Insertion Short

## Soru 1 : Yukarııda verilen dizinin short türüne göre aşamalarını yazınız.

[22,27,16,2,18,6] => 1. Aşama (n)

[2,27,16,22,18,6] => 2. Aşama (n-1)

[2,6,16,22,18,27] => 3. Aşama (n-2)

[2,6,16,18,22,27] => 4. Aşama (1)

## Soru 2 : Big-O gösterimini yazınız.

n + (n-1) + (n-2) + 1 = n.(n+1)/2

(n^2 + n ) / 2 = O(n^2)

## Soru 3 : Time Complexity: Average case: Aradığınız sayının ortada olması, Worst case: Aradığınız sayının sonda olması, Best case: Aradığınız sayının dizinin en başında olması.

Average case:
    [2,6,16,18,22,27] => 16,18

Worst case:
    [2,6,16,18,22,27] => 27

Best case:
    [2,6,16,18,22,27] => 2

## Soru 4 : Dizi sıralandıktan sonra 18 sayısı hangi cese kapsamına girer.

    Bir önce soruda da belirtildiği gibi Average Case Kapsamına girer.

## Soru : [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

[7,3,5,8,2,9,4,15,6] => 1. Aşama (n)

[2,3,5,8,7,9,4,15,6] => 2. Aşama (n-1)

[2,3,4,8,7,9,5,15,6] => 3. Aşama (n-2)

[2,3,4,5,7,9,8,15,6] => 4. Aşama (n-3)    Şeklinde devam eder.

# Merge Sort

        [16,21,11,8,12,22]

## Soru 1 : Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

                                        [16,21,11,8,12,22]
                                        ///                 \\\
                                [16,21,11]                  [8,12,22]                   => 1. Aşama
                                    ///                         \\\
                            [16]    [21,11]                     [8]     [12,22]         => 2. Aşama
                                ///                                 \\\
                            [16]    [21]    [11]                [8]     [12]    [22]    => 3. Aşama
                            ///                                         \\\
                            [16]    [11,21]                     [8]     [12,22]         => 4. Aşama
                            ///                                         \\\
                            [11,16,21]                          [8,12,22]               => 5. Aşama
                                                ||||
                                                [8,11,12,16,21,22]                      => 6. Aşama

## Soru 2 : Big-O gösterimini yazınız.

Her aşamada o(n) gelir.
n = 2^x
logn = x
O(n logn)

# Binary Search

## Soru : [7,5,1,8,3,6,0,9,4,2] dizisinin Binary-Search-Tree aşamalarını yazınız.

Öncelikle dizi sıralayalım.

[0,1,2,3,4,5,6,7,8,9]

Root Değer = 5

Dengeli bir dağılım için;

Solunda = 3

Sağında = 7


                                                            5
                                                        ///     \\\
                                                    3               7
                                                ///                 \\\
                                            2   4   6   8
                                            ///                         \\\
                                        1                                   9
                                        ///                             
                                    0

www.patika.dev Veri Yapıları ve Algoritmalar dersi proje ödevidir.