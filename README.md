# C# Notları
## Giriş
### Program.cs ve Main fonksiyonu
Uygulamanın başlangıç noktasıdır. Uygulama Program.cs dosyasının içerisindeki Main fonksiyonu ile başlar.

```c#
using System

namespace Test

    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello world!");
        }
    }
```
### Top-Level Statements
Using ve namespace arasında yazılabilen basit programlardır.

```c#
using System

Console.WriteLine("Hello world!");
```

### Yorum satırları
Yorum satırları kodlara açıklama yazmaya yarar.
```c#
using System

namespace Test

    class Program
    {
        static void Main(string[] args)
        {
            //Tek satırlık yorum
            Console.WriteLine("Hello world!");
        }
    }
```
```c#
using System

namespace Test

    class Program
    {
        static void Main(string[] args)
        {
            /*
            Çok
            satırlı
            yorum
            */
            Console.WriteLine("Hello world!");
        }
    }
```

### region
Region kodları kategorize etmemizi sağlar
```c#
using System

namespace Test

    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello world!");
        }
        
        #region X operasyonu
        
        #endregion
    }
```

### todo
Todo yapılan yorumların daha kolay bulunmasını sağlar. Todo ile yapılan yorumlara View/Task List menüsünden açılan ekrandan erişilebilir.
```c#
using System

namespace Test

    class Program
    {
        static void Main(string[] args)
        {
            //todo Merhaba Dünya
            Console.WriteLine("Hello world!");
        }
    }
```

## Değişkenler
### RAM Yapısı
**Stack :** Değer türlü değişkenlerin tutulduğu bölüm.
**Heap :** Nesnelerin tutulduğu bölüm.

**Değersiz Tanımlama :** degisken_tipi degisken_adi; Örnek int a;

**Değerli Tanımlama :** degisken_tipi degisken_adi = deger; Örnek int a = 5;
### Value Type
RAM'de alan tahsis edilen veri tipleridir. Örnek: string, int.
### Primitive Type
Türetilmemiş(ham) veri tipleridir. Örnek: byte
Primitive kontrolü aşağıdaki gibi yapılır.
```c#
using System

namespace Test

    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("typeof(decimal).IsPrimitive);
            Console.WriteLine("typeof(int).IsPrimitive);
            Console.WriteLine("typeof(byte).IsPrimitive);
        }
    }
```
### Veri Tipleri
**byte :** Uzunluğu 1 byte’tır, 0 ile 255 arasında değer alır.

**sbyte :** Uzunluğu 1 byte’tır, -128 ile 127 arasında değer alır.

**short :** Uzunluğu 2 byte’tır, -32768 ile 32767 arasında değer alır.

**ushort :** Uzunlupu 2 byte’tır, 0 ile 65535 arasında değer alır.

**int :** Uzunluğu 4 byte’tır, -2.147.483.648 ile 2.147.483.648 arasında değer alır.

**uint :** Uzunluğu 4 byte’tır, 0 ile 4.294.967.295 arasında değer alır.

**long :** Uzunluğu 8 byte’tır, -1020 ile 1020 arasında değer alır.

**ulong :** Uzunluğu 8 byte’tır, 0 ile 2 x 1020 arasında değer alır.

**float :** Uzunluğu 4 byte’tır, 1.5 x 10-45 ile 3.4 x 1038 arasında değer alır.

**double :** Uzunluğu 8 byte’tır, 5.0 x 10-324 ile 1.7 x 10308 arasında değer alır.

**decimal :** Uzunluğu 12 byte’tır, ±1.0 x 10-28 ile ±7.9 x 1028 arasında değer alır.

**char :** Uzunluğu 2 byte’tır, Bütün ınicode karakterleri kapsar.

**string :** Tek bir karakter, sözcük veya cümle gibi değerlerin saklanmasında kullanılır.

**boolean :** True – false değer tutan tiptir.
