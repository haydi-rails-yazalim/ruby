# Hafta 1

### Ruby
* Nesne Yönelimli
* Yorumlamalı
* Doğal dile yakın
* Açık kaynak geliştirilen
* Mutlu kod felsefesini benimseyen bir dil.

### RubyGems

* Ruby paketleme sistemi
* Farklı farklı kütüphanelerin yer aldığı
* Paketleri kurmak için kullanılan bir araç

### rbenv
* Ruby versiyonlarını yönettiğimiz
* Sürüm çakışması yaşamadan geçiş yapabildiğimiz bir paket.

### irb

* Ruby yorumlaycısını içeren
* Terminal'den 'irb' komutu ile başlayan
* Ruby kodlarını yorumlattığımız(çalıştırdığımız)
* ctrl + D veya exit ile çıktığımız bir paket.

#### Editor Seçimi
Kodlarımızın daha okunaklı görünmesi için tercih ettiğimiz araçlar.
* Atom
* Sublime
* Visual Studio Code
* Vim
* Emacs


#### Yorum Satırı
Ruby kodu yazdığımız .rb uzantılı dosyada, bilgilendirici fakat kodu etkilemeyen notlar bırakmak istediğimizde kullandığımız bir yöntem.

* #### Tek satır

  ```ruby
  #bu bir yorumdur fakat tek satırlı
  ```
* #### Çoklu satır

  ```ruby
  =begin
  çoklu
  satırlı
  yorum
  yazıyorum
  =end
  ```

#### Basit Matematiksel İşlemler
```ruby
(100/2)*1
=> 50

(30+20)-10
=> 40

2**4
=> 16
```

##### Değişkenler
###### Yerel
Tanımlanan blok içerisinde ulaşılabilirler.

```ruby
cemal = "hayat kısa"
sureya = "kuşlar uçuyor"

ruby_on_rails = 5
```

###### Örnek
Tanımlanan blok dışında da ulaşılabilirler.

```ruby
@uver = "Yaşayanlar seven sevene dünyada"
@cinka = "biz öldüğümüzle kalmıştık"

```

###### Sınıf
Sınıf içerisinde ulaşılabilirler.

```ruby
@@ucurumda = "Güzelsin sevgilim"
@@acan = "ama çok yakından"
```

###### Global
Her yerden ulaşılabilirler.

```ruby
$siir = "Kısa Türkiye Tarihi"
```

#### Puts, Print ve P
Ekrana yazdırmak için kullandığımız komutlar
```ruby
puts "life"
=> life

p "is"
=> "is"

p nil
=> nil

puts nil
=>

print "short"
print "birds"
=> shortbirds

puts "are"
=> are

puts "flying"
=> flying
```