# NOKTALARDAN-UZAKLIK-MATRISI-URETILMESI-VE-KNN-ALGORITMASI-ILE-SINIFLANDIRMA

1)
Genişliği (width) ve yüksekliği (height) verilen 2 boyutlu alan içerinde n adet rastgele nokta üreten ve döndüren metodu yazınız. 
Üretilen noktalar nx2 matris içerisinde; her bir satır bir noktaya ve her bir sütun da sırasıyla x ve y koordinat 
değerlerine karşılık gelecek biçimde saklanacak ve döndürülecektir. Üretilecek koordinatlar double tipinde olmalıdır.

Kendisine verilen nx2 noktalar
matrisini (bir önceki maddede istenen metot kullanılarak üretilmiş) nxn’lik uzaklık
matrisine çeviren ve döndüren metodu yazınız. Uzaklık matrisi (DM) her bir nokta çifti
arasındaki uzaklık bilgisini içermektedir. Örneğin, DM[i,j] i ve j noktaları arasındaki
mesafeyi verecektir. Uzaklıklar simetrik olduğundan DM[i,j]=DM[j,i] eşitliği sağlanacaktır
(i’den j’ye uzaklık ile j’den i’ye uzaklık aynıdır).

2)
Gerçek ve sahte banknot görüntü örneklerinden çıkarılan çeşitli öznitelikler bulunmaktadır. Bu
bilgiler aracılığı ile verilen görüntü gerçek/sahte olarak sınıflandırılabilmektedir. Her bir örnek
için 4’er adet özellik (varyans, çarpıklık, basıklık, entropi) bilgisi ve gerçek para olup/olmadığı
(tür) hazır olarak verilmektedir.Elimizde toplam 1372
adet örneğe ilişkin veriler bulunmaktadır. Bu verileri kullanarak, görüntünün iki farklı türden
hangisine ait olduğunu bulduran bir algoritmanın yazılması istenmektedir. Görüntü yerine
görüntü öznitelikleri kullanılarak işlemler gerçekleştirilecektir.

Bulduğumuz ancak türünü bilmediğimiz bir banknotun hangi türe ait olduğunu tespit eden algoritmayı (k en yakın komşu yöntemi) 
yazınız (hazır kNN kullanmayınız). k değerini, kullanıcı tarafından girilebilen bir banknotun tüm özellik(ler)ini girdi olarak 
aldırarak bu yöntemle hangi sınıftan (gerçek (1) / sahte (0)) olduğunu bulduran kNN algoritmasını kendiniz yazınız.

Yazdığınız kNN algoritmasının k değerini, kullanıcı tarafından girilebilen bir banknotun 4 adet özelliğini girdi olarak aldırarak, 
en yakın k adet banknotun özelliklerini, uzaklıklarını ve hangi sınıflardan olduklarını bir tablo olarak ekrana listeleyiniz. 
Bağlantısı önceki sayfada verilen verisetini kullanarak kNN yöntemi ile banknotun da türünü tahminleyiniz ve ekrana yazdırınız.

Verisetinde her bir tür banknot örneğinin sonunda yer alan 100’er veriyi
test verisi olarak ayırınız. k değerini kullanıcıdan aldırarak, test verilerinden herbirini, 4 özelliğin 
tümünü kullanarak kalan 1172 adet örnek veri üzerinden sınıflandırınız, Listelemeleri yapınız. Test verilerinin gerçek sınıfları ile, kNN ile
tahminlediğiniz sınıflarını karşılaştırınız (gerçek ve tahminlenen türlerin / sınıfların her ikisini de yazdırınız). 
Başarı oranını: doğru sınıflandırılan banknot sayısı / verisetinde test amaçlı kullandığınız toplam banknot sayısı
olarak hesaplayarak yazdırınız.
