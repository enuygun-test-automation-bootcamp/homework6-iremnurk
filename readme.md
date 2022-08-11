### ODEV

- [x] JAVA STREAM ÇALIŞILACAK
    - [x] JAVA STREAM NEDİR?
    - [x] STREAM MAP
    - [x] STREAM FILTER
    - [x] FOREACH
- [ ] flightTicketFromLiat metodundaki flightlist dizisi List'e çevrilecek stream kullanılarak
- [ ] checkListForSearch deki for döngüleri yerine stream kullanılacak
- [ ] Assertequals Key'e göre valueler getirip assertşion sağlanacak

* STREAM NEDİR
  
  Veri setleri deyince aklımıza ilk gelen veri yapıları Listeler veya Diziler olabilir. Java 8 ile birlikte gelen Stream Api desteği, veriler üzerinde yapacağımız işlemleri temiz ve anlaşılır bir şekilde ifade edebilmemize olanak sağlıyor.

* STREAM FILTER
  
  Filtre yöntemi, bağımsız değişken olarak iletilen Tahmine göre öğeleri seçmek için kullanılır.
  ```  List names = Arrays.asList("Reflection","Collection","Stream");
  List result = names.stream().filter(s->s.startsWith("S")).collect(Collectors.toList());
```      ```
 * Map

    Verilen işlevin bu akışın öğelerine uygulanmasının sonuçlarından oluşan bir akışı döndürmek için kullanılır. 

```List number = Arrays.asList(2,3,4,5);
List square = number.stream().map(x->x*x).collect(Collectors.toList());
```
* FOREACH
  
    For döngüsünde parantezlerin içerisine değer atama, başlangıç ve artım miktarı gibi ifadeler yazarız. Bunun yerine ForEach döngülerini kullanarak daha kısa ve basit bir şekilde döngü oluşturabiliriz.
```
String[] isimler = {"foreach","dongu","ders"};
        
        for(String i : isimler)
        {
            System.out.println(i);
        }
```