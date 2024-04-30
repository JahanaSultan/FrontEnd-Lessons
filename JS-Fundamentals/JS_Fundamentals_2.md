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

4. `charAt()`: Stringin verilmiş indeksindəki hərfi qaytarır. İndeks 0-dan başlayır.

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

18. `padStart()`: Stringin başına verilmiş simvolları əlavə edir.

```javascript
let text = "Hello";
console.log(text.padStart(10, ".")); // ".....Hello"
```

19. `padEnd()`: Stringin sonuna verilmiş simvolları əlavə edir.

```javascript
let text = "Hello";
console.log(text.padEnd(10, ".")); // "Hello....."
```

20. `at()`: Stringin verilmiş indeksindəki hərfi qaytarır. İndeks 0-dan başlayır.

```javascript
let text = "Hello";
console.log(text.at(1)); // "e"
```


## 3. String Şablonları (String Templates)

String şablonları, stringləri birləşdirmək üçün daha rahat bir yol təqdim edir. String şablonları `${}` işarələri arasında dəyişənləri və ya ifadələri yazmağa imkan verir. Məsələn:

```javascript
let name = "John";
let surname = "Doe";
let text = `Hello, ${name} ${surname}`;
console.log(text); // "Hello, John Doe"
```


## 4. Number Metodları (Number Methods)

Number tipli dəyişənlər üzərində aşağıdakı fərqli metodlar tətbiq edilə bilər:

1. `toString()`: Numberi stringə çevirir.

```javascript
let num = 5;
console.log(num.toString()); // "5"
```

2. `toFixed()`: Numberi verilmiş rəqəm qədər onluq ədədə çevirir. Lakin, bu metod yalnız string qaytarır.

```javascript
let num = 5.12345;
console.log(num.toFixed(2)); // "5.12"
```

3. `toPrecision()`: Numberi verilmiş rəqəm qədər onluq ədədə çevirir. Lakin, bu metod yalnız string qaytarır.

```javascript

let num = 5.12345;
console.log(num.toPrecision(2)); // "5.1"
```

4. `parseInt()`: Stringi onluq ədədə çevirir.

```javascript
let num = "5";
console.log(parseInt(num)); // 5
```

5. `parseFloat()`: Stringi onluq ədədə çevirir.

```javascript
let num = "5.12345";
console.log(parseFloat(num)); // 5.12345
```

6. `isNaN()`: Numberin `NaN` olub-olmadığını yoxlayır. `NaN` (Not a Number) ədəd olmayan bir dəyəri ifadə edir. 

```javascript
let num = 5;
console.log(isNaN(num)); // false
```

7. `isFinite()`: Numberin `Infinity` və ya `-Infinity` olub-olmadığını yoxlayır.

```javascript
let num = 5;
console.log(isFinite(num)); // true
```

8. `isInteger()`: Numberin tam ədəd olub-olmadığını yoxlayır.

```javascript
let num = 5;
console.log(Number.isInteger(num)); // true
```

9. `isSafeInteger()`: Numberin təhlükəsiz tam ədəd olub-olmadığını yoxlayır. Təhlükəsiz tam ədədlər, -2^53 və 2^53 aralığında olan tam ədədlərdir.

```javascript
let num = 5;
console.log(Number.isSafeInteger(num)); // true
```

10. `toExponential()`: Numberi eksponensial ədədə çevirir. Eksponensial ədədlər, ədədin rəqəmlərini və ədədin 10-cu ədədini ifadə edir. Məsələn, `5e+0` 5 ədədini ifadə edir.

```javascript
let num = 5;
console.log(num.toExponential()); // "5e+0"
```

11. `valueOf()`: Numberin dəyərini qaytarır.

```javascript
let num = 5;
console.log(num.valueOf()); // 5
```


## 5. Boolean Metodları (Boolean Methods)

Boolean tipli dəyişənlər üzərində aşağıdakı fərqli metodlar tətbiq edilə bilər:

1. `toString()`: Booleani stringə çevirir.

```javascript
let isStudent = true;
console.log(isStudent.toString()); // "true"
```

2. `valueOf()`: Booleanin dəyərini qaytarır.

```javascript
let isStudent = true;
console.log(isStudent.valueOf()); // true
```


## 6. Array Metodları (Array Methods)

Array tipli dəyişənlər üzərində aşağıdakı fərqli metodlar tətbiq edilə bilər:

1. `length`: Arrayin uzunluğunu qaytarır.

```javascript
let arr = [1, 2, 3];
console.log(arr.length); // 3
```

2. `push()`: Arrayin sonuna yeni element əlavə edir.

```javascript
let arr = [1, 2, 3];
arr.push(4);
console.log(arr); // [1, 2, 3, 4]
```

3. `pop()`: Arrayin sonundan element silir.

```javascript
let arr = [1, 2, 3];
arr.pop();
console.log(arr); // [1, 2]
```

4. `shift()`: Arrayin əvvəlindən element silir.

```javascript
let arr = [1, 2, 3];
arr.shift();
console.log(arr); // [2, 3]
```

5. `unshift()`: Arrayin əvvəlinə yeni element əlavə edir.

```javascript
let arr = [1, 2, 3];
arr.unshift(0);
console.log(arr); // [0, 1, 2, 3]
``` 

6. `concat()`: Arrayləri birləşdirir.

```javascript
let arr1 = [1, 2];
let arr2 = [3, 4];
let arr3 = arr1.concat(arr2);
console.log(arr3); // [1, 2, 3, 4]
```

7. `join()`: Arrayi stringə çevirir.

```javascript
let arr = [1, 2, 3];
console.log(arr.join()); // "1,2,3"
```

8. `reverse()`: Arrayin elementlərini tərsinə çevirir.

```javascript
let arr = [1, 2, 3];
arr.reverse();
console.log(arr); // [3, 2, 1]
```

9. `slice()`: Arrayin verilmiş indeksləri arasındakı elementləri qaytarır. İlk indeks daxil, ikinci indeks daxil deyil. İkinci indeks verilməsə, arrayin sonuna qədər olan elementləri qaytarır.

```javascript
let arr = [1, 2, 3, 4, 5];
console.log(arr.slice(1, 3)); // [2, 3]
```

10. `splice()`: Arraydən verilmiş indeksdən başlayaraq verilmiş sayda element silir və ya əlavə edir.

```javascript
let arr = [1, 2, 3, 4, 5];
arr.splice(1, 2);
console.log(arr); // [1, 4, 5]
```

11. `sort()`: Arrayi artan sıra ilə sıralayır.

```javascript
let arr = [3, 1, 2];
arr.sort();
console.log(arr); // [1, 2, 3]
```

Lakin, `sort()` metodu yalnız stringləri düzgün sıralayır. Əgər rəqəmləri düzgün sıralamaq istəyirsinizsə, sort metodu içində funksiya yazmalısınız. Məsələn:

```javascript
let arr = [3, 1, 2];
arr.sort((a, b) => a - b);
console.log(arr); // [1, 2, 3]
```

Əgər rəqəmləri azdan çoxa sıralamaq istəyirsinizsə, funksiyanın yerinə `-` işarəsini əvəz edin. Məsələn:

```javascript
let arr = [3, 1, 2];
arr.sort((a, b) => b - a);
console.log(arr); // [3, 2, 1]
```

12. `indexOf()`: Arraydə verilmiş elementin indeksini qaytarır. Əgər element tapılmazsa `-1` qaytarır. Birdən çox eyni element varsa, ilk tapılanın indeksini qaytarır.

```javascript
let arr = [1, 2, 3];
console.log(arr.indexOf(2)); // 1
```

13. `lastIndexOf()`: Arraydə verilmiş elementin sonuncu indeksini qaytarır. Əgər element tapılmazsa `-1` qaytarır. Birdən çox eyni element varsa, sonuncu tapılanın indeksini qaytarır.

```javascript
let arr = [1, 2, 3, 2];
console.log(arr.lastIndexOf(2)); // 3
```

14. `includes()`: Arraydə verilmiş elementin olub-olmadığını yoxlayır.

```javascript
let arr = [1, 2, 3];
console.log(arr.includes(2)); // true
```

15. `every()`: Arrayin bütün elementləri üçün verilmiş şərti yoxlayır. Əgər bütün elementlər şərti ödəyirsə `true`, əks halda `false` qaytarır.

```javascript
let arr = [1, 2, 3];
console.log(arr.every((element) => element > 0)); // true
```

16. `some()`: Arrayin hər hansı bir elementi üçün verilmiş şərti yoxlayır. Əgər hər hansı bir element şərti ödəyirsə `true`, əks halda `false` qaytarır.

```javascript
let arr = [1, 2, 3];
console.log(arr.some((element) => element > 2)); // true
```

17. `filter()`: Arraydə verilmiş şərtə uyğun elementləri qaytarır. Yeni array yaradır və şərtə uyğun olan elementləri bu arrayə əlavə edir.

```javascript
let arr = [1, 2, 3];
let newArr = arr.filter((element) => element > 1);
console.log(newArr); // [2, 3]
```

18. `map()`: Arraydə verilmiş funksiyanı hər bir elementə tətbiq edir. Yeni array yaradır və funksiyanın qaytardığı dəyərləri bu arrayə əlavə edir.

```javascript
let arr = [1, 2, 3];
let newArr = arr.map((element) => element * 2);
console.log(newArr); // [2, 4, 6]
```

19. `reduce()`: Arraydə verilmiş funksiyanı elementlərə tətbiq edir və bir dəyər qaytarır. Məsələn, elementləri toplamaq üçün `reduce()` metodu istifadə olunur.

```javascript
let arr = [1, 2, 3];
let sum = arr.reduce((total, element) => total + element, 0);
console.log(sum); // 6
```

20. `find()`: Arraydə verilmiş şərtə uyğun ilk elementi qaytarır. Əgər element tapılmazsa `undefined` qaytarır. Yalnız bir element qaytarır.

```javascript
let arr = [1, 2, 3];
let element = arr.find((element) => element > 1);
console.log(element); // 2
```

21. `findIndex()`: Arraydə verilmiş şərtə uyğun ilk elementin indeksini qaytarır. Əgər element tapılmazsa `-1` qaytarır. Yalnız bir elementin indeksini qaytarır.

```javascript
let arr = [1, 2, 3];
let index = arr.findIndex((element) => element > 1);
console.log(index); // 1
```

22. `forEach()`: Arrayin hər bir elementinə verilmiş funksiyanı tətbiq edir. Yeni array yaratmır.

```javascript
let arr = [1, 2, 3];
arr.forEach((element) => console.log(element));
```


# Dərs 2 Tapşırıqlar

