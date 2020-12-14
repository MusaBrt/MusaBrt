Yeni başlayanların anlaması için yazılmış bir yazı.

# Methodlar nedir
Methodlar içerisinde dışardan parametre alabilen kod parçacıklarıdır. Çalıştıktan sonra çalıştırıldığı yere herhangi bir veri verebilir. Mesela boolean dönderen bir methodu çalıştırırsan sana ya true ya da false dönderir. Bazı durumlarda bu true false ile işlemler yaptırabilirsin. Örneğin string'i sayıya çevireceğin zaman kontrol etmek isteyebilirsin. kontrolEt(string) şeklindeki bir boolean dönderen methodu çalıştırırsın. Method false dönderirse demek ki sayı olamıyor, içinde harf var.

Örnekler:
```java
public void methodum() {
  // herhangi bir veri döndermeyen ve parametre almayan bir methodum isimli method. Aynı sınıf içinde methodum(); şeklinde kullanılabilir.
}```

```java
public boolean methodum(String text) {
   // içine text değişken ismiyle String tipinden parametre alan bir methodum isimli method. Geriye boolean dönderiyor. Void methodda return kullanmak zorunda değiliz. Kullanırsak 'return;' şeklinde kullanabilirsin. Bu direkt methodu kullandığın yerde bitirir. Fakat geriye bir veri dönderen methodlarda zorunlu olarak veri döndermek zorundasın.
  return false;
   // hata almamak için boş methodda false dönderdik. true'da dönderilebilir keyfe kalmış.
}```

`Son Örnek:` Rastgele hasar almak için bu methodu üst sınırı belirterek aynı sınıf içerisinde kullanabilirsin. Tüm sınıflardan kullanmak için methodunun static olması gerekiyor. Static methodlar içinde static olmayan nesnelere erişemez, kullanamazsın. Bunun belli başlı sebepleri var. İlerledikten sonra öğrenebilirsin.

```java
public int rastgeleHasarAl(int maksimum) {
  Random random = new Random();
  return random.nextInt(maksimum);
}```
