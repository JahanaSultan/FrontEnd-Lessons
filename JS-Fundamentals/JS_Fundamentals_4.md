# Javascript Dərs 4

## Funksialar (Functions)

Funksiya, müəyyən bir tapşırığı yerinə yetirmək üçün hazırlanmış yenidən istifadə edilə bilən kod bloku və ya proqramlaşdırma ifadələridir. Funksiya, funksiya açar sözü ilə təyin olunur və ardınca ad, sonra da mötərizələr `()` gəlir. Mötərizələrin içində funksiyaya bir parametr ötürə bilərik. Funksiya kodu:

- Təmiz və oxunaqlı edir
- Yenidən istifadə edilə bilər
- Test etmək asandır

Funksiya bir neçə yolla təyin edilə bilər:

- Declaration function
- Expression function
- Anonymous function
- Arrow function

Funksialar, aşağıdakı sintaksis ilə təyin olunur:

```javascript
function funksiyaAdı(parametr1, parametr2, ...) {
    // Funksiya daxilində icra olunacaq əməliyyatlar
    return dəyər;
}

// Funksiya çağırılır
funksiyaAdı(arg1, arg2, ...);
```

Funksiyalar parametr qəbul etmədən və dəyər qaytarmadan da yaradıla bilər:

```javascript
function funksiyaAdı() {
  // Funksiya daxilində icra olunacaq əməliyyatlar
  console.log("Funksiyanı işə saldınız");
}

// Funksiya çağırılır
funksiyaAdı(); // "Funksiyanı işə saldınız"
```

Anonim funksiyalar (Anonymous function): Bu funksiyalar adı olmayan funksiyalardır. Çox zaman funksiya ifadələri və ya callback funksiyalar olaraq istifadə olunurlar

```javascript
let funksiyaAdı = function(parametr1, parametr2, ...) {
    // Funksiya daxilində icra olunacaq əməliyyatlar
    return dəyər;
}

// Funksiya çağırılır
funksiyaAdı(arg1, arg2, ...);
```

Arrow funksiyalar: Arrow funksiyalar, ES6 ilə daxil olmuşdur. Arrow funksiyalar, funksiya ifadələrini qısaltmaq üçün istifadə olunur.

```javascript
let funksiyaAdı = (parametr1, parametr2, ...) => {
    // Funksiya daxilində icra olunacaq əməliyyatlar
    return dəyər;
}

// Funksiya çağırılır
funksiyaAdı(arg1, arg2, ...);
```

Expression funksiyalar : Bu tip funksiyalar bir dəyişkənə mənimsədilir. Bu funksiyaları ancaq özündən aşağıdakı sətirlərdə istifadə etmək mümkündür:

```javascript
let funksiyaAdı = function(parametr1, parametr2, ...) {
    // Funksiya daxilində icra olunacaq əməliyyatlar
    return dəyər;
}

// Funksiya çağırılır
funksiyaAdı(arg1, arg2, ...);
```

Declaration funksiyalar: Bu tip funksiyalar yazıldığı sətirdən üst sətirlərdə də çağırıla bilərlər və bu xüsusiyyətə `hoisting` deyilir:

```javascript
// Funksiya təyin olunur
function funksiyaAdı(parametr1, parametr2, ...) {
    // Funksiya daxilində icra olunacaq əməliyyatlar
    return dəyər;
}

// Funksiya çağırılır
funksiyaAdı(arg1, arg2, ...);
```

Funksiyaların parametr qəbul etməsi və dəyər qaytarması məcbur deyil. Funksiya parametr qəbul etməsə, mötərizələr içində heç bir şey yazılmır. Funksiya dəyər qaytarmırsa, `return` ifadəsi istifadə etmək məcbur deyil. Funksiya dəyər qaytarmırsa, `undefined` dəyərini qaytarır.

Funsiyalarda parametrlərə default dəyər vermək mümkündür:

```javascript
function greetings(istifadeciAdi = "Istifadeci") {
  let salamlama = `Xos geldin ${istifadeciAdi}`;
  return salamlama;
}

console.log(greetings()); // "Xos geldin Istifadeci"
console.log(greetings("Gunes")); // "Xos geldin Gunes"
```

## Array Metodları (Array Methods)

Dəyişənlərdən fərqli olaraq, Array birdən çox dəyəri saxlaya bilər. Hər bir dəyərin Arraydə indeksi var və hər bir indeksin bir yaddaş ünvanı var. Hər bir dəyər indeksləri istifadə edərək əldə edilə bilər. Arrayin indeksi sıfırdan başlayır və son elementin indeksi arrayin uzunluğundan bir azdır.

Array, düzgün sıralanmış və dəyişdirilə bilən fərqli data tiplərinin bir qrupudur. Array, eyni elementləri və fərqli data tiplərini saxlamağa imkan verir. Array boş ola bilər və ya fərqli data tipi dəyərlərə malik ola bilər.

JavaScript-də Array yaratmaq üçün fərqli yollar mövcuddur. Array dəyişənini təyin etmək üçün `let` əvəzinə `const` istifadə etmək çox yaygındır. Əgər `const` istifadə edirsinizsə, bu dəyişən adını daha sonra istifadə etməyəcəyinizi göstərir.

- `Array()` konstruktor vasitəsi ilə:

```javascript
let arr = new Array();
```

- `[]` köşəli mötərizələr vasitəsi ilə:

```javascript
let arr = [];
```

- Elementlərlə birlikdə:

```javascript
let arr = [1, 2, 3];
```

Arrayin elementlərinə müraciət etmək üçün indeksləri istifadə edirik. Indekslər sıfırdan başlayır. Məsələn, birinci elementə müraciət etmək üçün indeks 0-dır.

```javascript
const arr = [1, 2, 3];
console.log(arr[0]); // 1
```

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

23. `flat()`: Arraydə verilmiş dərəcədə olan arrayləri düz arrayə çevirir.

```javascript
let arr = [1, [2, 3], 4];
let newArr = arr.flat();
console.log(newArr); // [1, 2, 3, 4]
```

24. `flatMap()`: Arraydə verilmiş dərəcədə olan arrayləri düz arrayə çevirir və verilmiş funksiyanı hər bir elementə tətbiq edir.

```javascript
let arr = [1, [2, 3], 4];
let newArr = arr.flatMap((element) => element * 2);
console.log(newArr); // [2, 4, 6, 8]
```

25. `from()`: Arraydən yeni array yaradır.

```javascript
let arr = [1, 2, 3];
let newArr = Array.from(arr);
console.log(newArr); // [1, 2, 3]
```

26. `isArray()`: Verilmiş dəyərin array olub-olmadığını yoxlayır.

```javascript
let arr = [1, 2, 3];
console.log(Array.isArray(arr)); // true
```

27. `keys()`: Arrayin indekslərini qaytarır.

```javascript
let arr = [1, 2, 3];
let keys = arr.keys();
for (let key of keys) {
  console.log(key); // 0, 1, 2
}
```

28. `values()`: Arrayin dəyərlərini qaytarır.

```javascript
let arr = [1, 2, 3];
let values = arr.values();
for (let value of values) {
  console.log(value); // 1, 2, 3
}
```

29. `entries()`: Arrayin indekslərini və dəyərlərini qaytarır.

```javascript
let arr = [1, 2, 3];
let entries = arr.entries();
for (let entry of entries) {
  console.log(entry); // [0, 1], [1, 2], [2, 3]
}
```

30. `fill()`: Arrayin verilmiş indekslərini verilmiş dəyərlərlə doldurur.

```javascript
let arr = [1, 2, 3];
arr.fill(0, 1, 2);
console.log(arr); // [1, 0, 3]
```

31. `copyWithin()`: Arrayin verilmiş indekslərini verilmiş indeksə kopyalayır.

```javascript
let arr = [1, 2, 3, 4, 5];
arr.copyWithin(0, 3, 4);
console.log(arr); // [4, 2, 3, 4, 5]
```

# Dərs 4 Tapşırıqlar

1. `helloWorld` adında funksiya yaradın və hər dəfə çağırıldığında "Salam Dünya" yazısını ekrana çıxarsın.
2. `greetUser` adında funksiya yazın və istifadəçinin adını və soyadını parametr olaraq qəbul edib hər çağırıldığında müxtəlif istifadəçiləri salamlasın.
3. `calculate` adında funksiya yaradın, iki ədəd və işarə qəbul etsin. Hesablamanın nəticəsini `return` etsin
4. `isEven` adında funksiya yazın və bir rəqəm qəbul edib ədəd cütdürsə `true`, əks halda `false` qaytarsın.
5. `isOdd` adında funksiya yazın və bir rəqəm qəbul edib ədəd təkdirsə `true`, əks halda `false` qaytarsın.
6. `isPrime` adında funksiya yazın və bir rəqəm qəbul edib ədəd sadədirsə `true`, əks halda `false` qaytarsın.
7. `fibonacci` adında funksiya yazın və bir rəqəm qəbul edib fibonacci ardıcıllığının n-ci elementini qaytarsın.
8. `areaOfRectangle` adında funksiya yaradın və kvadratın enini və uzununu parametr olaraq qəbul etsin və düzbucaqlının sahəsini `return` etsin.
9. `areaOfCircle` adında funksiya yaradın və radiusu parametr olaraq qəbul etsin və dairənin sahəsini `return` etsin.
10. `checkSeason` adında funksiya yaradın və ayı parametr olaraq göndərin. Hansı mövsüm olduğunu `return` etsin.
11. `sumOfPrimeNumbers` adında funksiya yaradın və iki ədəd parametr olaraq göndərin. Funksiya iki ədəd arasındakı sadə ədədlərin cəmini `return` etsin.
12. `reverseString` adında funksiya yaradın və bir string qəbul etsin və stringi tərsinə çevirsin.
13. `isPalindrome` adında funksiya yaradın və bir string qəbul etsin və string palindromdur (tərsinə oxuna bilərsə) `true`, əks halda `false` qaytarsın.
14. `findLongestWord` adında funksiya yaradın və bir string qəbul etsin və ən uzun sözü `return` etsin.
15. `findShortestWord` adında funksiya yaradın və bir string qəbul etsin və ən qısa sözü `return` etsin.
16. `findVowels` adında funksiya yaradın və bir string qəbul etsin və stringdə olan samitlərin sayını `return` etsin.
17. 2 array yaradın və uzunluqlarını müqayisə edin.
18. Bir array yaradın və arrayın ən başda ən sonda və ortada olan elementini çap edin (ortada tək element yoxdursa iki element çap edin)
19. Bir array yaradın və arrayin elementlərini tərsinə çevirin.
20. Bir array yaradın və arrayin elementlərini artan sıra ilə sıralayın.
21. Bir array yaradın və arrayin elementlərini azalan sıra ilə sıralayın.
22. Bir array yaradın və arrayin elementlərini toplayın.
23. Bir array yaradın və arrayin elementlərinin cüt və tək olanlarını ayırın.
24. Bir array yaradın və arrayin elementlərinin sadə və mürəkkəb olanlarını ayırın.
25. Bir array yaradın və arrayin elementlərinin ədəd olub-olmadığını yoxlayın. Başqa arraydə eyni sıra ilə ədəd olan `true` olmayan `false` ilə təmsil olunsun.
26. Aşağıdakı array üzərində qeyd olunan əməliyyatları aparın.

```javascript
const countries = [
  "Azerbaijan",
  "Albania",
  "Bolivia",
  "Canada",
  "Denmark",
  "Ethiopia",
  "Finland",
  "Germany",
  "Hungary",
  "Ireland",
  "Japan",
  "Kenya",
];
```

- Arrayin uzunluğunu tapın
- Arrayin sonuna "Norway" əlavə edin
- Arrayin əvvəlinə "Turkey" əlavə edin
- Arrayin 3-cü elementini silin
- Arrayin 5-ci elementini dəyişin
- Arrayin 2-ci elementini tapın
- Arrayin son elementini tapın
- Arrayin "Germany" elementinin indeksini tapın
- Arrayin sonuncu elementini silin
- Arrayin əvvəlindəki 3 elementi silin
- Arrayin 5 ci elementini "Sudan" ilə əvəz edin
- Arrayin əvvəlindəki 3 elementi "USA", "UK", "UAE" ilə əvəz edin

27. Aşağıdakı array üzərində qeyd olunmuş əməliyyatları yerinə yetirin:

```javascript
const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]
```

- Ən böyük və ən kiçik ədədi tapın
- Ədədlərin ortalamasını tapın
- Ədədlərin cəmini tapın
- Ədədlərin cüt və tək olanlarını ayırın
- Ədədlərin sadə və mürəkkəb olanlarını ayırın

28. Arrayda olan dublikat elemetləri silib unik elemetlərdən ibarət yeni array yaradın.

```javascript
const numbers = [1, 2, 3, 4, 4, 5, 6, 6, 7, 8, 9, 9];
```
29. Bir array yaradın və arrayin bütün metodlarını tək-tək test edin.