# İsim uzayları (Namespaces)

- Programlama dillerinde bir takım hazır kütüphaneler mevcuttur.  Bu kütüphanelerin bazıları standart olmasının yanı sıra bazıları da programcılar tarafından oluşturulmuştur. Genel olarak Nesne Tabanlı (Object Oriented) programlama dillerinde (Visual Basic, Java, C++,...gibi) hazır kütüphanelerden faydalanılır. Fakat C# dilinde standart bir  kütüphane bulunmamaktadır. Bu durum yazılım açısından işleri daha da kolaylaştırır. Bu konuda Microsoft’un geliştirdiği .NET Framework adlı bir alt yapı kullanılmaktadır. Bu alt yapı Microsoft’un geliştirdiği programlama dillerini kullanan programcılara temel türler ve sınıflar sunmuştur. .Net bütün bu sınıfları ve türleri iyi bir şekilde organize edebilmek için  isim uzayı (namespace) kavramını sıklıkla kullanır. İsim uzayları (namespaces) şu şekilde tanımlanır:

namespace Test
{
    class Sinif
    {
        //kod
    }
}

- İsim uzayları (Namespaces) C# dilinde  using  anahtar sözcüğü ile kullanılır, fakat isim uzayları (namespaces)  diğer dillerde  farklı şekillerde derleyiciye bildirilseler de bütün Nesne Tabanlı (Object Oriented) programlama dillerinde yapılan iş aynıdır. Şu şekilde isim uzayları (namespaces) programa eklenir:

using Test;

- Bir yazılımcı yazdığı kodların organizasyonunda isim uzaylarını (namespaces) kullanabilir. Tür ismi ya da sınıf sadece  kendi isim uzayları (namespaces) içinde görünürlüğe sahip olduğundan isim uzaylarının (namespaces) kullanılması tür isimlerinin ya da sınıf isimlerinin karışmasını engeller. Yazılan sınıflar  için de bir isim uzayı (namespace)  tanımlanarak kaynak kod istenilen şekilde organize edilebilir. Ayrıca .Net Framework ile içiçe (nested) isim uzayları (namespaces) tanımlanmıştır. Böylece yazılımcı hazırladığı kodları çok daha rahat organize edebilmektedir. İçiçe (nested) isim uzayları (namespaces) ile hiyerarşik bir düzene sahip kod blokları yaratılır; bu da yazılımcının işini oldukça kolaylaştırmaktadır. İçiçe (nested) isim uzayları (namespaces) şu şekilde tanımlanır:

namespace Test
{
    namespace Test2
    {
        class Sinif
        {
            //kod
        }
    }
}

- İçiçe (nested) isim uzayları (namespaces) programa eklenirken de "using" anahtar sözcüğü kullanılır. Tek fark içteki bir isim uzayı (namespace) kullanılmak istendiğinde "using" anahtar sözcğüyle birlikte isim uzayının (namespace) tam yolu yazılmalıdır. Şu şekilde örneklendirilebilir:

using Test.Test2;
