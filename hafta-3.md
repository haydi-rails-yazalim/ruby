# Hafta 3

### Döngüler
Tekrar tekrar kullanılabilen kod blokları.

```ruby
5.times { print "Hello"}
=> "HelloHelloHelloHelloHello"

a = 2
3.times { a *= 2 }
puts a
=> 16

b = 3
while b <= 4
  puts "ben #{b} yaşındayım"
  b +=1
end
=> "ben 3 yasşındayım"
=> "ben 4 yasşındayım"

for c in 1..3
  puts "Sen #{c}. misin?"
end
=> "Sen 1. misin?"
=> "Sen 2. misin?"
=> "Sen 3. misin?"

@a = []
(0..2).each do |n|
  @a << n
end
puts @a
=> [0, 1, 2]
```

### Metotlar
Belli bir görevi olan kod bloğu. Programın farklı yerlerinden çağırılabilirler. Ruby'de metotların son satırı döner.

```ruby
def method_name
  # parametre almayan metodun gövdesi
end

def method_name(param1, param2, param3)
  # 3 parametre alan metodun gövdesi
end

def carpma(a, b)
  puts a * b
end
carpma(5, 10) #iki parametreli metodun çağırısı
=> 50

def toplama(one, *other)
  sum = 0
  other.each { |n| sum += n }
  sum + one
end
puts toplama(3,4,12,24) # one = 3, other = [4, 12, 24] (parametrelerin alacağı değerler)
=> 43
```