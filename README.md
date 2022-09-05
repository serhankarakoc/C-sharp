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
### Value Type
RAM'de alan tahsis edilen veri tipleridir. Örnek: string, int.
### Primitive Type
Türetilmemiş(ham) veri tipleridir. Örnek: byte
