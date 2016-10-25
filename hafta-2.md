# Hafta 2

### Sabitler
Büyük harf ile başlamalı ve isteğe göre büyük harfle devam edebilir. Ayrıca Sabitler ruby'de o kadar da sabit değillerdir :)

```ruby
LIFE = "hayat"
LIFE = "ömür"
=> warning: already initialized constant AL
=> warning: previous definition of AL was here

puts LIFE
=> ömür
```

### Semboller
Stringlere benzerler En büyük farkları bir kere oluşturulduklarında o adresi her zaman korurlar.


```ruby
name = :life
name.object_id
=> 2435228

surname = :life
surname.object_id
=> 2435228

name.inspect
=> ":life"

ktu = "zor hayat"
defined?(ktu)
=> "local-variable"

defined?(:life)
=> "expression"
```

### Basit Girdi Çıktı İşlemleri

```ruby
name = gets.chomp
puts name

life = "yaşam"
life.chop
=>"yaşa"

life.chomp
=>"yaşam"

age = gets.chomp.to_i
age += 1
puts age
```

### Diziler
Verileri sakladığımız bir yapıdır. İçlerinde farklı tipler yer alabilir.

```ruby
meyveler = ["elma", "armut", "çilek"]
meyveler.methods #dizi ile kullanabileceğim metotları sıralar

meyveler[-1]
=>çilek

meyveler.first
=>elma

meyveler.length
=>3

meyveler.pop
=>["elma", "armut"]

meyveler.push("ananas")
=>["elma","armut","ananas"]

meyveler << "kivi"
=>["elma","armut","ananas","kivi"]

everything = [34, "istanbul", :gezgin]
```

### Mantıksal İfadeler

```ruby
10 == 10.0
=>true

age, hop, life = 20, "hop", :hayat # paralel atama
age <= 19 && "hop" == hop || :life == :hayat
=>false
```

### Akış Kontrolü

```ruby
anil = 10
irem = 12

if irem < anil
  puts "anıl irem'den büyüktür"
elsif anil < irem
  puts "irem anıl'den büyüktür"
else
  puts "anil ile irem aynı yaştadır."
end
=>"irem anıl'dan büyüktür"

puts 1 <= 5 ? "doğru" : "yanlış"
=>"doğru"

while anil < irem
  puts "anıl #{anil} yaşında ve hala irem'den küçük"
  anil += 1
end
=>"anıl 10 yaşında ve hala irem'den küçük"
=>"anıl 11 yaşında ve hala irem'den küçük"
```