# Patika Insertion Sort-Projesi - Proje1
##### Bu repo [Patika](http://www.patika.dev) sitesi Veri Yapıları ve Algoritmalar dersi Projeler bölümünde bulunan Insertion Sort Projesi - Proje 1 çalışması için oluşturulmuştur.


>[22,27,16,2,18,6] -> Insertion Sort
1.Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

Algoritmada dizi en baştan sona doğru sıralı olarak ilerler. İlk olarak birinci eleman ikinci elemanın büyüklükleri kıyaslanır. İkinci eleman birinci elemandan küçük ise sıralamaları değiştirilir. İkinci elemanın değeri büyükse sıralama değişmez ardından üçüncü elemana geçilir. İşlem tüm dizideki elemanlar bitene kadar bu şekilde sırayla devam eder.

#### Adım 1

| 22 | 27 | 16 | 2 | 18 | 6 |
| :---: | :---: | :---: |:---: | :---: | :---: |

 22 ile 27 elemanı arasında karşılaştırma yapılır. 22, 27 den küçük olduğu için sıralama değişikliği yapılmaz.



#### Adım 2

|22|  27 | 16 | 2 | 18 | 6 |  > | 22	|16	|27	|2 | 18 |  6 | > | 16	|22	|27|	2	|  18|	6|
| :---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: |:---: |


16, 27 elemanlarının büyüklük kıyaslaması yapılır ve aralarında sıralama değişikliği olur. Daha sonra 16 elemanı yer değiştirdikten sonra solundaki eleman bakar ve kendinden büyük ya da küçük olup olmadığını kıyaslar. 16, 22 den küçük olduğu için aralarında 22 nin sol tarafına geçer.

#### Adım 3

|16|	22|	2|	 27|	 18|  6|  >|16|	 2 |  22 |	27|	18|	6   |>|	2	|  16|	22|	27|	18|	6|
| :---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: |:---: | 

2, büyüklük kıyaslamasında küçük olduğu için sırayle 27, 22 ve 16 ile yer değiştirir.

#### Adım 4

|2|	  16|	22|	18|	27|	6	|  >	|  2 |  16|	18|	22|	27|	6|
| :---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: |:---: | :---: | :---: |:---: | :---: |

18, büyüklük kıyaslamasında küçük olduğu için sırayla 27, 22 ile değiştirir ancak 16 dan büyük olduğu için dizindeki sıralaması sonlandırılır.

#### Adım 5

|2|	  16|	18|	22|	6|	  27|	>	|2|	  16|	18|	6| 	22|	27|   >|  
| :---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: | :---: |

|     2|	  16|	6 |	18	|22	|27	|  > | 	2 |	6 |	16	|18|	22|	27| 
| :---: |:---: | :---: | :---: |:---: |:---: | :---: | :---: |:---: | :---: | :---: |:---: |:---: |

6, büyüklük kıyaslamasında küçük olduğu için sırayla 27, 22, 18, 16 ile yer değiştirir ancak 2 den büyük olduğu için dizindeki sıralaması sonlandırılır.



>2.Big-O gösterimini yazınız.
```
O(n^2)
```


>3.Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
```
Worst Case: O(n^2) 

Avarage Case: O(n^2) 

Best Case: O(n)
```



>4.Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız. 

Average case



[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

1.Adım	
|7|	3|	  5|	  8| 	2|	  9|	  4|	  15|  	6|
| :---: | :---: |:---: |:---: | :---: | :---: |:---: | :---: | :---: |

2.Adım	
|3|	7|	  5|	  8| 	2| 	9 |	4 	|15  	|6|
| :---: | :---: |:---: |:---: | :---: | :---: |:---: | :---: | :---: |

3.Adım	
|3|	5|	  7|	  8| 	2| 	9 |	4 	|15  	|6|
| :---: | :---: |:---: |:---: | :---: | :---: |:---: | :---: | :---: |

4.Adım	
|3|	5|	  7|	  8| 	2| 	9 |	4 	|15  	|6|
| :---: | :---: |:---: |:---: | :---: | :---: |:---: | :---: | :---: |
