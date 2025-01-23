# Libft - 42 Cursus Projesi

Libft, 42 Cursus'ta C dilinde bir standart kütüphane oluşturmayı amaçlayan temel bir projedir. Bu proje ile C dilindeki standart fonksiyonların yeniden yazılması ve ek fonksiyonların oluşturulması hedeflenmiştir.

## İçerik

Bu kütüphane, aşağıdaki fonksiyonları ve yapıları içerir:

### Standart Fonksiyonlar

#### Karakter Kontrol Fonksiyonları
- `ft_isalpha`: Bir karakterin alfabetik olup olmadığını kontrol eder.
- `ft_isdigit`: Bir karakterin rakam olup olmadığını kontrol eder.
- `ft_isalnum`: Bir karakterin harf ya da rakam olup olmadığını kontrol eder.
- `ft_isascii`: Bir karakterin ASCII olup olmadığını kontrol eder.
- `ft_isprint`: Bir karakterin yazdırılabilir olup olmadığını kontrol eder.
- `ft_toupper`: Küçük harfi büyük harfe dönüştürür.
- `ft_tolower`: Büyük harfi küçük harfe dönüştürür.

#### String İşleme Fonksiyonları
- `ft_strlen`: Bir stringin uzunluğunu hesaplar.
- `ft_strncmp`: İki stringi belirli bir uzunluğa kadar karşılaştırır.
- `ft_strchr`: Bir karakterin string içindeki ilk konumunu bulur.
- `ft_strrchr`: Bir karakterin string içindeki son konumunu bulur.
- `ft_strnstr`: Bir alt stringi belirli bir uzunlukta arar.
- `ft_strdup`: Bir stringin kopyasını oluşturur.
- `ft_strlcpy`: Bir stringi kopyalar.
- `ft_strlcat`: Bir stringi başka bir stringin sonuna ekler.
- `ft_substr`: Bir stringin bir alt kısmını döndürür.
- `ft_strjoin`: İki stringi birleştirir.
- `ft_strtrim`: Belirli karakterleri kırparak bir string döndürür.
- `ft_strmapi`: Bir stringin her karakterine belirli bir fonksiyonu uygular.
- `ft_split`: Bir stringi belirli bir ayırıcıya göre böler.

#### Bellek Yönetimi Fonksiyonları
- `ft_memset`: Belleği belirli bir değerle doldurur.
- `ft_bzero`: Belleği sıfırlar.
- `ft_memcpy`: Belleğin bir kısmını başka bir yere kopyalar.
- `ft_memmove`: Belleğin bir kısmını güvenli bir şekilde taşır.
- `ft_memchr`: Bellekte belirli bir değeri arar.
- `ft_memcmp`: Belleğin iki kısmını karşılaştırır.
- `ft_calloc`: Dinamik bellek ayırır ve sıfırlar.

#### Dönüştürme Fonksiyonları
- `ft_atoi`: Bir stringi tam sayıya dönüştürür.
- `ft_itoa`: Bir tam sayıyı stringe dönüştürür.

#### Giriş/Çıkış Fonksiyonları
- `ft_putchar_fd`: Bir karakteri belirli bir dosya tanıtıcısına yazar.
- `ft_putstr_fd`: Bir stringi belirli bir dosya tanıtıcısına yazar.
- `ft_putendl_fd`: Bir stringi yeni bir satırla birlikte yazar.
- `ft_putnbr_fd`: Bir tam sayıyı belirli bir dosya tanıtıcısına yazar.

### Bonus Fonksiyonlar

Libft projesinin bonus kısmı, bağlantılı liste yapısını ve bu yapı üzerinde işlem yapan fonksiyonları içerir. Bonus kısmında tanımlanan `t_list` yapısı ve fonksiyonlar şunlardır:

#### Yapı
- `t_list`: Bağlantılı liste için bir düğüm yapısını tanımlar. Bu yapı şu alanlardan oluşur:
  - `content`: Düğümün taşıdığı veri.
  - `next`: Bir sonraki düğüme işaretçi.

#### Liste Fonksiyonları
- `ft_lstnew`: Yeni bir düğüm oluşturur.
- `ft_lstadd_front`: Listenin başına yeni bir düğüm ekler.
- `ft_lstadd_back`: Listenin sonuna yeni bir düğüm ekler.
- `ft_lstdelone`: Belirtilen düğümü siler ve belleği serbest bırakır.
- `ft_lstclear`: Listedeki tüm düğümleri siler ve belleği serbest bırakır.
- `ft_lstiter`: Listenin her düğümüne belirli bir fonksiyonu uygular.
- `ft_lstsize`: Listedeki düğüm sayısını döndürür.
- `ft_lstlast`: Listenin son düğümünü döndürür.
- `ft_lstmap`: Belirli bir fonksiyonu kullanarak yeni bir liste oluşturur.

## Kullanım

Kütüphaneyi kullanabilmek için aşağıdaki adımları takip edebilirsiniz:

1. **Proje Build İşlemi**
   ```bash
   make
   ```
   Bu komut, `libft.a` adlı statik kütüphaneyi oluşturur.

2. **Kütüphaneyi Projeye Dahil Etme**
   `libft.a` dosyasını kendi projenize aşağıdaki gibi ekleyebilirsiniz:
   ```c
   #include "libft.h"
   ```

3. **Compile İşlemi**
   ```bash
   gcc -Wall -Wextra -Werror main.c libft.a -o output
   ```

## Gereksinimler

- `gcc` veya benzeri bir C derleyicisi.
- `Makefile` ile uyumlu bir build ortamı.

## Lisans

Bu proje, 42 Network lisans kurallarına tabidir.
