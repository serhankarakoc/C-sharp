# C#
## Program.cs ve Main fonksiyonu
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
## Top-Level Statements
Using ve namespace arasında yazılabilen basit programlardır.

```c#
using System

Console.WriteLine("Hello world!");
```

## Yorum satırları - region - todo
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
