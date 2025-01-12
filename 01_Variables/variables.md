# Değişkenler ve Sabitler

Sabitler ve değişkenler bir adı (piSayisi veya welcomeMessage gibi) belirli bir türdeki bir değerle (3.14 sayısı veya "Hello" dizesi gibi) ilişkilendirir. Bir sabitin değeri ayarlandıktan sonra değiştirilemezken, bir değişken gelecekte farklı bir değere ayarlanabilir.

Gerçek programlar her seferinde aynı çıktıyı vermek yerine program kullanıcısının verdiği bazı girdilere dayalı sonuçlar üretme eğilimindedir. Değişken bilgisayarın belleğinde veri saklamamız, almamız ve kullanmamız için ayrılmış belirli bir parçayı temsil eden yapıdır.

Her değişkenin içinde saklayabileceğimiz bilgi türünü temsil eden bir tipi vardır. Bu tip bilgisi derleyiciye ne kadar bellek ayırması gerektiğini söyler. Bu veri türü değişken sınırlarını belirler.

```swift
import UIKit

var mesaj = "Merhaba, Swift"
```

Sabitlerin ve değişkenlerin kullanılmadan önce bildirilmesi gerekir. Sabitleri let anahtar sözcüğü ile değişkenleri ise var anahtar sözcüğü ile bildiririz.

Örneğin bir kullanıcın uygulamamıza giriş yaptığında hatalı girişlerini takip edip belli bir değere ulaştıktan sonra güvenlik önlemi olarak belli bir süre giriş denemesi yapmasına engel olmak istediğimizi varsayalım. Bu noktada kullanıcının oturum açma hakkını bir sabit olarak ayarlayabiliriz. Kullanıcın oturum açma denemelerini de değişken olarak ayarlayabiliriz. Kullanıcı her oturum açma denemesinde hata yaptığında değişken değeri bir artırılarak sabite ulaştığında önlemi devreye alabiliriz.

## Değişken ve Sabit Tanımlama Yöntemleri

1. Veri türünü belirtmeden başlangıç değeri vererek tanımlayabiliriz.

   ```swift
   var sayi = 5
   ```

2. Veri türünü belirtip başlangıç değeri vermeden tanımlayabiliriz.

   ```swift
   var sayi: Int
   sayi = 10
   print(sayi)
   ```

3. Veri türü ve başlangıç değeri vererek tanımlayabiliriz.

   ```swift
   var sayi: Int = 5
   print(sayi)
   ```

Tek bir satırda virgülle ayırarak birden fazla sabit veya birden fazla değişken bildirebiliriz.

```swift
var sayi1 = 0, sayi2 = 10, sayi3 = 20
```

Bir sabit veya değişken tanımlarken saklayabileceği veri türünü belirtebiliriz.

```swift
var mesaj: String = "Merhaba"
var sayi: Int = 5
```

Sabit ya da değişkeni içinde saklayacağı veri türü ile bildirdiğimizde başlangıç değeri atama zorunluluğumuz yoktur. Yine aynı türde birden fazla değişkeni tek bir satırda, virgülle ayırarak ve son değişken adından sonra tek bir tür ek açıklamasıyla tanımlayabiliriz.

```swift
let piSayisi: Double
var a, b, c: Float
```

Bir sabit ya değişken tanımladığımızde veri türünü belirtmezsek başlangıç değerinin türü ne ise veri türü olarak onu kabul eder. Daha sonra değişkene farklı türde bir değer atadığımızda hata verecektir.

![Ekran Resmi 2025-01-12 15.28.55](/Users/smhmurat/Library/Application Support/typora-user-images/Ekran Resmi 2025-01-12 15.28.55.png)

Sabit ya da değişken isimlendirmelerinde dikkat edilecek kurallar:

- Sabit ya da değişken ismi rakam ile başlayamaz. İlk karakter dışındaki karakterleri rakam olabilir.
- Sabit ya da değişken isimleri operatör (+, -, *, /, vb.) içeremez. Sadece alt çizgi (_) karakteri içerebilir.
