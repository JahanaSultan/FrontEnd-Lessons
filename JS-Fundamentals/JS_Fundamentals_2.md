# Javascript Dərs 2

## 1. Data Tipləri (Data Types)

Data tipləri, dəyişənlərin nə qədər yer tutduğunu və dəyişənlərin hansı növ məlumatları saxladığını göstərir. Javascript-in əsas data tipləri aşağıdakılardır:

1. String
2. Number
3. Bigint
4. Boolean
5. Undefined
6. Null
7. Symbol
8. Object

Dəyişkənin data tipini öyrənmək üçün `typeof` operatorundan istifadə olunur. Məsələn:

```javascript
let name = "Javascript";
console.log(typeof name); // "string"
```

### 1.1. String

String, mətn tipli dəyişənləri ifadə edir. String dəyişənləri tək və ya cüt dırnaq işarələri arasında yazılır. Məsələn:

```javascript
let name = "Javascript";
let surname = "Dərs";
```

String dəyişənlərində dırnaq işarələri arasında başqa dırnaq işarəsi istifadə etmək üçün `escape` işarələrindən istifadə olunur. Məsələn:

```javascript
let text = "I'm a student";
let text2 = 'He said: "Hello"';
```

### 1.2. Number

Number, rəqəm tipli dəyişənləri ifadə edir. Məsələn:

```javascript
let age = 25;
let pi = 3.14;
```

Javascript-in Number tipli dəyişənləri ədədlər, onluq ədədlər, onaltılıq ədədlər və eksponensial ədədlər kimi fərqli növlərdə olur. Məsələn:

```javascript
let num1 = 123; // ədəd
let num2 = 0.123; // onluq ədəd
let num3 = 0x123; // onaltılıq ədəd
let num4 = 1.23e3; // eksponensial ədəd
```

Javascript-in Number tipli dəyişənləri üzərində riyazi əməliyyatlar aparmaq mümkündür. Məsələn:

```javascript
let x = 5;
let y = 3;
let z = x + y; // 8
let w = x * y; // 15
let q = x / y; // 1.6666666666666667
let r = x % y; // 2
```

Javascriptdə bütün ədədlər onluq ədədlər kimi saxlanılır. Number tipli dəyişənləri string tipli dəyişənlərlə birləşdirmək üçün `+` operatorundan istifadə olunur. Bu zaman Number tipli dəyişənlər string tipli dəyişənlərə çevrilir. Məsələn:

```javascript
let num = 5;
let text = "Number is: " + num; // "Number is: 5"
```

### 1.3. Bigint

Bigint, böyük rəqəmləri ifadə etmək üçün istifadə olunur. Məsələn:

```javascript
let bigNumber = 1234567890123456789012345678901234567890n;
```

### 1.4. Boolean

Boolean, iki dəyəri ifadə edir: `true` və `false`. Məsələn:

```javascript
let isStudent = true;
let isTeacher = false;
```

Hər zaman `true` olan dəyərlər (truthy values):

1. 0 dan başqa bütün pozitiv və neqativ rəqəmlər.
2. `""` bo. stringd'n başqa bütün stringlər.
3. Bütün obyektlər.
4. `true` dəyəri.
5. `Infinity` dəyəri.

Hər zaman `false` olan dəyərlər (falsy values):

1. 0
2. `NaN`.
3. `null`.
4. `undefined`.
5. `false`.
6. `''` (boş string).

### 1.5. Undefined

Undefined, dəyişənin dəyərinin təyin edilmədiyini ifadə edir. Məsələn:

```javascript
let x;
console.log(x); // undefined
```

### 1.6. Null

Null, dəyişənin dəyərinin boş olduğunu ifadə edir. Məsələn:

```javascript
let y = null;
console.log(y); // null
```

### 1.7. Symbol

Symbol, dəyişənləri unikal olaraq təyin etmək üçün istifadə olunur. Məsələn:

```javascript
let id = Symbol("id");
```

### 1.8. Object

Object, obyektləri ifadə edir. Obyekt, açar-dəyər cütlüyündən ibarət bir məlumat strukturudur. `{}` işarələri arasında açar-dəyər cütlükləri yazılır. Məsələn:

```javascript
let student = {
  name: "John",
  surname: "Doe",
  age: 25,
};
```

## 2. String Metodları (String Methods)

Metodlar, dəyişənlər üzərində fərqli əməliyyatlar aparmağa imkan verir. String tipli dəyişənlər üzərində aşağıdakı fərqli metodlar tətbiq edilə bilər:

1. `length`: Stringin uzunluğunu qaytarır.

```javascript
let text = "Hello";
console.log(text.length); // 5
```

2. `toUpperCase()`: Stringi böyük hərflərə çevirir.

```javascript
let text = "Hello";
console.log(text.toUpperCase()); // "HELLO"
```

3. `toLowerCase()`: Stringi kiçik hərflərə çevirir.

```javascript
let text = "Hello";
console.log(text.toLowerCase()); // "hello"
```

4. `charAt()`: Stringin verilmiş indeksindəki hərfi qaytarır. İndeks 0-dan başlayır. `[indeks]` operatoru ilə eyni funksiyonu yerinə yetirir.

```javascript
let text = "Hello";
console.log(text.charAt(1)); // "e"
```

5. `indexOf()`: Stringdə verilmiş substringin indeksini qaytarır. Əgər substring tapılmazsa `-1` qaytarır. Birdən çox eyni substring varsa, ilk tapılanın indeksini qaytarır.

```javascript
let text = "Hello";
console.log(text.indexOf("l")); // 2
```

6. `lastIndexOf()`: Stringdə verilmiş substringin sonuncu indeksini qaytarır. Əgər substring tapılmazsa `-1` qaytarır. Birdən çox eyni substring varsa, sonuncu tapılanın indeksini qaytarır.

```javascript
let text = "Hello";
console.log(text.lastIndexOf("l")); // 3
```

7. `includes()`: Stringdə verilmiş substringin olub-olmadığını yoxlayır.

```javascript
let text = "Hello";
console.log(text.includes("l")); // true
```

8. `startsWith()`: Stringin verilmiş substring ilə başlayıb-başlamadığını yoxlayır.

```javascript
let text = "Hello";
console.log(text.startsWith("H")); // true
```

9. `endsWith()`: Stringin verilmiş substring ilə bitib-bitmədiyini yoxlayır.

```javascript
let text = "Hello";
console.log(text.endsWith("o")); // true
```

10. `slice()`: Stringin verilmiş indeksləri arasındakı substringi qaytarır. İlk indeks daxil, ikinci indeks daxil deyil. İkinci indeks verilməsə, stringin sonuna qədər olan substringi qaytarır.

```javascript
let text = "Hello";
console.log(text.slice(1, 3)); // "el"
```

11. `substring()`: Stringin verilmiş indeksləri arasındakı substringi qaytarır. İlk indeks daxil, ikinci indeks daxil deyil. `slice()` metodundan fərqi, `substring()` metodunda indekslər dəyişəndən kiçikdən böyük olmalıdır. İkinci index verilməsə, stringin sonuna qədər olan substringi qaytarır.

```javascript
let text = "Hello";
console.log(text.substring(1, 3)); // "el"
```

12. `substr()`: Stringin verilmiş indeksindən başlayaraq verilmiş uzunluqda substringi qaytarır.

```javascript
let text = "Hello";
console.log(text.substr(1, 3)); // "ell"
```

13. `replace()`: Stringdə verilmiş substringi digər substring ilə əvəzləyir. Yalnız ilk tapılan substringi əvəzləyir. `replaceAll()` metodu ilə bütün substringləri əvəzləyə bilərsiniz.

```javascript
let text = "Hello";
console.log(text.replace("l", "w")); // "Hewlo"
console.log(text.replaceAll("l", "w")); // "Hewwo"
```

14. `split()`: Stringi verilmiş simvola görə ayırır.

```javascript
let text = "Hello";
console.log(text.split("")); // ["H", "e", "l", "l", "o"]
```

15. `trim()`: Stringin ətrafındakı boşluqları silir.

```javascript
let text = " Hello ";
console.log(text.trim()); // "Hello"
```

16. `repeat()`: Stringi verilmiş sayda təkrar edir.

```javascript
let text = "Hello";
console.log(text.repeat(3)); // "HelloHelloHello"
```

17. `concat()`: Stringləri birləşdirir.

```javascript
let text1 = "Hello";
let text2 = "World";
console.log(text1.concat(" ", text2)); // "Hello World"
```

18. `padStart()`: Stringin başına uzunluğu tamamlayacaq sayda əlavə etmək istədiyimiz simvolu əlavə edir. Yəni stringin uzunluğu verilmiş uzunluğa çatana qədər simvol əlavə edir. Əgər stringin uzunluğu verilmiş uzunluğdan böyük olarsa, stringi dəyişdirmir.

```javascript
let text = "Hello";
console.log(text.padStart(10, ".")); // ".....Hello"
```

19. `padEnd()`: Stringin sonuna uzunluğu tamamlayacaq sayda əlavə etmək istədiyimiz simvolu əlavə edir. Yəni stringin uzunluğu verilmiş uzunluğa çatana qədər simvol əlavə edir. Əgər stringin uzunluğu verilmiş uzunluqdan böyük olarsa, stringi dəyişdirmir.

```javascript
let text = "Hello";
console.log(text.padEnd(10, ".")); // "Hello....."
```

20. `at()`: Stringin verilmiş indeksindəki hərfi qaytarır. İndeks 0-dan başlayır.

```javascript
let text = "Hello";
console.log(text.at(1)); // "e"
```

21. `match()` : Bu metod vasitəsi ilə verilmiş stringdə verilmiş regex-i axtarır və uyğunluqları array şəklində qaytarır. Əgər uyğunluq tapılmazsa `null` qaytarır.
  
  ```javascript
  let text = "Hello";
  console.log(text.match("l")); // ["l", "l"]
  ```

22. `search()` : Bu metod bir string içərisində bir ifadəni (regex) axtarır. 
  Əgər taparsa, tapdığı indeksi qaytarır. Əgər tapmazsa `-1` qaytarır.
  
  ```javascript
  let text = "Hello";
  console.log(text.search("l")); // 2

  let text2 ="Mən javascripti sevirəm"
  console.log(text2.search("javascript")); // 4
  console.log(text2.search(/Javascript/gi)) // 4 (Burada g və i regex in iki flag(bayrağını) təmsil edir. g - Global axtarış bayrağıdır. Bu bayraq, uyğunlaşma tapılsada stringin hamısında axtarmağa davam edir. i - Böyük / kiçik hərf həssaslığının olmamasını bildirir. Yəni axtarılan sözün böyük və ya kiçik hərflərlə yazılmasından asılı olmayaraq tapılmasını təmin edir.)
  ```

## 3. Dəyişənlərin tiplərini yoxlama

Dəyişənlərin tiplərini yoxlamaq üçün `typeof` metodundan istifadə olunur. Məsələn:

```javascript
let name = "John";
let age = 25;
let isStudent = true;
let job;

console.log(typeof name); // "string"
console.log(typeof age); // "number"
console.log(typeof isStudent); // "boolean"
console.log(typeof job); // "undefined"
console.log(typeof NaN) // number
console.log(typeof null) // object
```

## 4. String Şablonları (String Templates)

String şablonları, stringləri birləşdirmək üçün daha rahat bir yol təqdim edir. String şablonları `${}` işarələri arasında dəyişənləri və ya ifadələri yazmağa imkan verir. Məsələn:

```javascript
let name = "John";
let surname = "Doe";
let text = `Hello, ${name} ${surname}`;
console.log(text); // "Hello, John Doe"
```

# Dərs 2 Tapşırıqlar

1. Bir neçə dəyişkən elan et və həmin dəyişkənlərin data tiplərini `typeof` operatoru ilə ekrana çap et.
2. İki string dəyişkən elan et və bu dəyişkənləri birləşdirərək yeni bir dəyişkənə mənimsə. Nəticəni ekrana çap et.
3. Verilmiş stringin uzunluğunu ekrana çap et.
4. Verilmiş stringin verilmiş indeksindəki hərfi ekrana çap et.
5. Verilmiş stringdə verilmiş substringin indeksini ekrana çap et.
6. Verilmiş stringdə verilmiş substringin sonuncu indeksini ekrana çap et.
7. Verilmiş stringdə verilmiş substringin olub-olmadığını ekrana çap et.
8. Verilmiş stringin verilmiş substring ilə başlayıb-başlamadığını ekrana çap et.
9. Verilmiş stringin verilmiş substring ilə bitib-bitmədiyini ekrana çap et.
10. Verilmiş stringin verilmiş indeksləri arasındakı substringi ekrana çap et.
11. Verilmiş stringin verilmiş indeksindən başlayaraq verilmiş uzunluqda substringi ekrana çap et.
12. Verilmiş stringdə verilmiş substringi digər substring ilə əvəzləyərək nəticəni ekrana çap et.
13. Verilmiş stringi verilmiş simvola görə ayıraraq nəticəni ekrana çap et.
14. Verilmiş stringin ətrafındakı boşluqları silərək nəticəni ekrana çap et.
15. Verilmiş stringi verilmiş sayda təkrar edərək nəticəni ekrana çap et.
16. Verilmiş stringləri birləşdirərək nəticəni ekrana çap et.
17. Verilmiş stringin başına uzunluğu tamamlayacaq sayda əlavə etmək istədiyimiz simvolu əlavə edərək nəticəni ekrana çap et.
18. Verilmiş stringin sonuna uzunluğu tamamlayacaq sayda əlavə etmək istədiyimiz simvolu əlavə edərək nəticəni ekrana çap et.
19. Verilmiş stringin içində hər hansı subsrtingin olub-olmadığını yoxla və onu dəyişərək nəticəni ekrana çap et.