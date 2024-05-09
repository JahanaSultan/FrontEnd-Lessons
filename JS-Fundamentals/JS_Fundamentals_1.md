# Javascript Dərs 1

## Javascript haqqında qısa məlumat

Javascript dünyanın ən populyar proqramlaşdırma dillərindən biridir. Javascript-in əsas məqsədi veb səhifələrə interaktivlik əlavə etməkdir. Yəni, Javascript-in köməyi ilə səhifədə olan elementlərə müdaxilə edə bilərik. Öyrənməsi asandır.

## Javascript-in əsas xüsusiyyətləri

1. **Dynamik**: Javascript-in əsas xüsusiyyətlərindən biri də dinamik olmasıdır. Yəni, səhifədə olan elementlərə müdaxilə edə bilərik. Məsələn, səhifədə olan bir elementin rəngini dəyişdirmək, elementi gizlətmək və s. Javascript-in köməyi ilə bunları asanlıqla həyata keçirə bilərik.

2. **Asinxron**: Javascript asinxron proqramlaşdırma dilidir. Yəni, Javascript-in kodları səhifədən yuxarı aşağı işləmir. Javascript-in kodları eyni anda işləmir. Məsələn, bir funksiya işlədikdə, digər funksiya işləmir. Bu da Javascript-in asinxron olmasının əsas səbəbidir.

3. **Sadə**: Javascript sadə bir proqramlaşdırma dilidir. Javascript-in sintaksisi sadədir. Yəni, Javascript-in sintaksisi başqa proqramlaşdırma dillərinə nisbətən sadədir. Bu da Javascript-in öyrənilməsini asanlaşdırır.

4. **Əlaqə**: Javascript-in əsas məqsədi veb səhifələrə interaktivlik əlavə etməkdir. Yəni, Javascript-in köməyi ilə səhifədə olan elementlərə müdaxilə edə bilərik. Bu da Javascript-in əlaqəli olmasının əsas səbəbidir.

## Javascript-in tarixi

Javascript 1995-ci ildə Brendan Eich tərəfindən yaradılmışdır. Javascript-in adı Java ilə heç bir əlaqəsi yoxdur. Javascript-in adı Java ilə yanaşıldığı üçün, insanlar Javascript-i Java ilə eyni proqramlaşdırma dili kimi düşünür. Lakin, Javascript-in Java ilə heç bir əlaqəsi yoxdur. Javascript-in adı Java ilə yanaşıldığı üçün, Javascript-in adı ECMAScript olaraq dəyişdirilmişdir. Javascript-in əsas versiyaları ECMAScript 3, ECMAScript 5, ECMAScript 6, ECMAScript 7, ECMAScript 8, ECMAScript 9, ECMAScript 10, ECMAScript 11, ECMAScript 12-dir.

## Javascript file necə yaradılır?

Javascript fayllarını `.js` uzantılı fayllar ilə yarada bilərik. Məsələn, `script.js` adlı bir fayl yaradaq. Faylın adı istədiyiniz ola bilər. Faylın adını yaratdıqdan sonra, bu faylı HTML faylına əlavə edərək, Javascript kodlarını burada yazaraq, səhifədə olan elementlərə müdaxilə edə bilərik.
Htmldə script faylını əlavə etmək üçün aşağıdakı kodu yazmaq kifayətdir:

```html
<script src="script.js"></script>
```

Bu kodu yazdıqdan sonra, `script.js` faylında olan Javascript kodları səhifədə işləyəcək.

## Javascript də dataları göstərmək

Javascript-də dataları göstərmək üçün 4 əsas metoddan istifadə edə bilərik. Bunlar:

1. **alert()**: Dataları ekranda göstərmək üçün `alert()` və ya `window.alert()` metodundan istifadə edə bilərik. Məsələn, aşağıdakı kodu yazdıqda, ekranda `Salam, Javascript!` mesajı göstəriləcək:

```javascript
alert("Salam, Javascript!");
```

2. **innerHTML**: Dataları HTML elementlərinin daxilində göstərmək üçün `innerHTML` metodundan istifadə edə bilərik. Məsələn, aşağıdakı kodu yazdıqda, `p` elementinin daxilində olan mətn dəyişəcək:

```html
<p id="demo">Salam, HTML!</p>

<script>
  document.getElementById("demo").innerHTML = "Salam, Javascript!";
</script>
```

3. **console.log()**: Dataları konsolda göstərmək üçün `console.log()` metodundan istifadə edə bilərik. Məsələn, aşağıdakı kodu yazdıqda, konsolda `Salam, Javascript!` mesajı göstəriləcək. Test məqsədləri üçün istifadə edə bilərsiniz:

```javascript
console.log("Salam, Javascript!");
```

4. **document.write()**: Dataları səhifədə göstərmək üçün `document.write()` metodundan istifadə edə bilərik. Məsələn, aşağıdakı kodu yazdıqda, səhifədə `Salam, Javascript!` mətni göstəriləcək. Bu metodun əsas xüsusiyyəti, səhifədə olan digər elementləri silməsidir. Yəni, `document.write()` metodunu işlətdikdə, səhifədə olan digər elementlər silinəcək. Bu metoddan istifadə etmək üçün, aşağıdakı kodu yazmaq kifayətdir. Bu metodu yalnız test məqsədləri üçün istifadə edə bilərsiniz:

```javascript
document.write("Salam, Javascript!");
```

## Javascript şərh yazmaq

Javascript-də şərh yazmaq üçün `//` və ya `/* */` işarələrindən istifadə edə bilərik. Məsələn, aşağıdakı kodda, `//` işarəsi ilə şərh yazılmışdır:

```javascript
// Bu şərh sətiri tək sətirlik şərh yazmaq üçündür

/* Bu şərh sətiri
çoxlu sətirlərdə
şərh yazmaq üçündür */
```

Qısayol: `Ctrl + /`, `Ctrl + ?` (windows) və ya `Cmd + /`, `Cmd + ?`(mac) düymələrinə eyni anda basaraq, seçdiyiniz kodları şərhə çevirə bilərsiniz. Eyni zamanda `Ctrl + /` (windows) və ya `Cmd + /` (mac) düymələrinə eyni anda basaraq, şərhə çevrilmiş kodları normallaşdıra bilərsiniz.

## Javascript dəyişənlər

Js-də dəyişənlər, məlumatları saxlamaq üçün istifadə olunur. Dəyişənlərə məlumatları saxlamaq üçün `var`, `let` və ya `const` açar sözlərindən istifadə edə bilərik. Bu açar sözlərini bir növ elan edici şəxs olaraq düşünə bilərsiniz. Yəni js də program və dəyişkəni bir biri ilə tanış edən vasitəçi rolunu oynayır. Dəyişənlərə məlumatları saxlamaq üçün aşağıdakı sintaksisi istifadə edə bilərik:

```javascript
var ad = "Fərhad";
let soyad = "Quluzadə";
const yas = 20;
```

Yuxarıdakı kodda, `ad` dəyişəninə `Fərhad`, `soyad` dəyişəninə `Quluzadə`, `yas` dəyişəninə isə `20` məlumatı mənimsədilmişdir. `var` açar sözü ilə dəyişənlər global dəyişənlər kimi istifadə olunur. `let` açar sözü ilə dəyişənlər isə yalnız o blok daxilində istifadə olunur. `const` açar sözü ilə dəyişənlər isə dəyişəninə məlumat mənimsədildikdən sonra, dəyişəninə başqa məlumat mənimsədə bilməzsiniz.

`var` və `let` açar sözləri arasındakı fərqi aşağıdakı nümunədə göstərək:

```javascript
{
  var ad = "Fərhad";
  let soyad = "Quluzadə";
}

console.log(ad); // Fərhad
console.log(soyad); // Uncaught ReferenceError: soyad is not defined
```

Yuxarıdakı kodda, `var` açar sözü ilə dəyişənlər global dəyişənlər kimi istifadə olunur. `let` açar sözü ilə dəyişənlər isə yalnız o blok daxilində istifadə olunur. Bu da `soyad` dəyişəninə blok daxilində olduğu üçün, konsolda `Uncaught ReferenceError: soyad is not defined` xətası göstərilir.

`const` və `let` açar sözləri arasındakı fərqi aşağıdakı nümunədə göstərək:

```javascript
const yas = 20;
yas = 25; // Uncaught TypeError: Assignment to constant variable.
```

Bu kodda, `const` açar sözü ilə mənimsədilmiş dəyişəninə başqa məlumat mənimsədə bilməzsiniz. Bu da `Uncaught TypeError: Assignment to constant variable.` xətasını göstərir. Lakın, `let` açar sözü ilə mənimsədilmiş dəyişəninə başqa məlumat mənimsədə bilərsiniz.

`var` açar sözü 1995 - 2015-ci illərdə istifadə olunurdu. Lakin, 2015-ci ildə ECMAScript 6 ilə birlikdə `let` və `const` açar sözləri də əlavə olundu. Bu açar sözlər `var` açar sözündən daha təhlükəsizdir. Bu açar sözləri istifadə etmək daha məsləhətdir.

Dəyişənlərin adlandırılmasında bir neçə qayda var:

1. Dəyişənlər hər zaman kiçik hərflərlə yazılır.
2. Birdən çox söz olan dəyişənlər _ işarələri ilə yazılır. Məsələn, `ad_soyad`.
3. Dəyişənlər rəqəmlə başlaya bilməz.
4. Dəyişənlər özel simvollar ilə başlaya bilməz.
5. Dəyişənlərin adında boşluq olmaz.
6. Dəyişənlər təkrar olmamalıdır.

Dəyişənlərin adlandırılmasında istifadə edilməməsi gərəkən adlar aşağıdakılardır:

1. `break`
2. `case`
3. `catch`
4. `class`
5. `const`
6. `continue`
7. `debugger`
8. `default`
9. `delete`
10. `do`
11. `else`
12. `export`
13. `extends`
14. `finally`
15. `for`
16. `function`
17. `if`
18. `import`
19. `in`
20. `instanceof`
21. `new`
22. `return`
23. `super`
24. `switch`
25. `this`
26. `throw`
27. `try`
28. `typeof`
29. `var`
30. `void`
31. `while`
32. `with`
33. `yield`


## Javascript operatorlar

Js-də operatorlar, dəyişənlər arasında riyazi əməliyyatlar etmək üçün istifadə olunur. Operatorlar, dəyişənlər arasında toplama, çıxma, vurma, bölmə və s. əməliyyatlar etmək üçün istifadə olunur. Js-də əsas operatorlar aşağıdakılardır:

1. **Toplama operatoru (+)**: Dəyişənlər arasında toplama əməliyyatı etmək üçün istifadə olunur. Məsələn, aşağıdakı kodda, `a` və `b` dəyişənlərinin cəmini konsolda göstərəcəyik:

```javascript
var a = 5;
var b = 10;
var c = a + b;
console.log(c); // 15
```

2. **Çıxma operatoru (-)**: Dəyişənlər arasında çıxma əməliyyatı etmək üçün istifadə olunur. Məsələn, aşağıdakı kodda, `a` və `b` dəyişənlərinin fərqini konsolda göstərəcəyik:

```javascript
var a = 10;
var b = 5;
var c = a - b;
console.log(c); // 5
```

3. **Vurma operatoru (*)**: Dəyişənlər arasında vurma əməliyyatı etmək üçün istifadə olunur. Məsələn, aşağıdakı kodda, `a` və `b` dəyişənlərinin hasilini konsolda göstərəcəyik:

```javascript
var a = 5;
var b = 10;
var c = a * b;
console.log(c); // 50
```

4. **Bölmə operatoru (/)**: Dəyişənlər arasında bölmə əməliyyatı etmək üçün istifadə olunur. Məsələn, aşağıdakı kodda, `a` və `b` dəyişənlərinin nəticəsini konsolda göstərəcəyik:

```javascript
var a = 10;
var b = 5;
var c = a / b;
console.log(c); // 2
```

5. **Modulus operatoru (%)**: Dəyişənlər arasında modulus əməliyyatı etmək üçün istifadə olunur. Yəni, iki ədədin bölünməsindən qalıqı göstərmək üçün istifadə olunur. Məsələn, aşağıdakı kodda, `a` və `b` dəyişənlərinin qalığını konsolda göstərəcəyik:

```javascript
var a = 10;
var b = 3;
var c = a % b;
console.log(c); // 1
```

6. **Artırma operatoru (++)**: Dəyişənin dəyərini bir vahid artırmaq üçün istifadə olunur. Əvvəldə yazıldıqda əvvəlcə dəyəri artırır daha sonra göstərir:

```javascript
let a=5;
console.log(++a); // 6
```
Sonrasında yazıldıqda isə əvvəlcə göstərir daha sonra dəyəri artırır:

```javascript
let a=5;
console.log(a++); // 5
console.log(a); // 6
```

7. **Azaltma operatoru (--)**: Dəyişənin dəyərini bir vahid azaltmaq üçün istifadə olunur. Əvvəldə yazıldıqda əvvəlcə dəyəri azaldır daha sonra göstərir:

```javascript
let a=5;
console.log(--a); // 4
```
Sonrasında yazıldıqda isə əvvəlcə göstərir daha sonra dəyəri azaldır:

```javascript
let a=5;
console.log(a--); // 5
console.log(a); // 4
```

8. **Qüvvət operatoru (**)**: Dəyişənlərin qüvvətini hesablamaq üçün istifadə olunur. Məsələn, aşağıdakı kodda, `a` və `b` dəyişənlərinin qüvvətini konsolda göstərəcəyik:

```javascript
var a = 2;
var b = 3;
var c = a ** b;
console.log(c); // 8
```

9. **Birləşdirmə operatoru (+)**: Dəyişənləri birləşdirmək üçün istifadə olunur. Məsələn, aşağıdakı kodda, `a` və `b` dəyişənlərini birləşdirdikdə, konsolda `Javascript` mətni göstəriləcək:

```javascript
var a = "Java";
var b = "script";
var c = a + b;
console.log(c); // Javascript
```


## Javascript təyin operatorları

Js-də təyin operatorları, dəyişənlərə məlumat mənimsətmək üçün istifadə olunur. Js-də əsas təyin operatorları aşağıdakılardır:

1. **Təyin operatoru (=)**: Dəyişənlərə məlumat mənimsətmək üçün istifadə olunur. Məsələn, a dəyişəninə `5` məlumatını mənimsədək:

```javascript
var a = 5;
```

2. **Toplama təyin operatoru (+=)**: Dəyişənin dəyərinə əlavə məlumat mənimsəmək üçün istifadə olunur. Məsələn, a dəyişəninə `5` məlumatını mənimsədikdən sonra, `a` dəyişəninə `10` əlavə məlumatını mənimsədək:

```javascript
var a = 5;
a += 10; // a = a + 10

console.log(a); // 15
```

3. **Çıxma təyin operatoru (-=)**: Dəyişənin dəyərindən çıxmaq üçün istifadə olunur. Məsələn, a dəyişəninə `10` məlumatını mənimsədikdən sonra, `a` dəyişənindən `5` çıxmaq üçün istifadə olunur:

```javascript
var a = 10;
a -= 5; // a = a - 5

console.log(a); // 5
```

4. **Vurma təyin operatoru (*=)**: Dəyişənin dəyərinə vurmaq üçün istifadə olunur. Məsələn, a dəyişəninə `5` məlumatını mənimsədikdən sonra, `a` dəyişənini `10` vurmaq üçün istifadə olunur:

```javascript
var a = 5;
a *= 10; // a = a * 10

console.log(a); // 50
```

5. **Bölmə təyin operatoru (/=)**: Dəyişənin dəyərini bölmək üçün istifadə olunur. Məsələn, a dəyişəninə `10` məlumatını mənimsədikdən sonra, `a` dəyişənini `5` bölmək üçün istifadə olunur:

```javascript
var a = 10;
a /= 5; // a = a / 5

console.log(a); // 2
```

6. **Modulus təyin operatoru (%=)**: Dəyişənin dəyərini modulus etmək üçün istifadə olunur. Məsələn, a dəyişəninə `10` məlumatını mənimsədikdən sonra, `a` dəyişənini `3` modulus etmək üçün istifadə olunur:

```javascript
var a = 10;
a %= 3; // a = a % 3

console.log(a); // 1
```

7. **Qüvvət təyin operatoru (**=)**: Dəyişənin dəyərini qüvvətləmək üçün istifadə olunur. Məsələn, a dəyişəninə `2` məlumatını mənimsədikdən sonra, `a` dəyişənini `3` qüvvətləmək üçün istifadə olunur:

```javascript
var a = 2;
a **= 3; // a = a ** 3

console.log(a); // 8
```

## Javascript müqayisə operatorları

Js-də müqayisə operatorları, dəyişənlər arasında müqayisə etmək üçün istifadə olunur. Js-də əsas müqayisə operatorları aşağıdakılardır:

1. **Bərabərlik operatoru (==)**: Dəyişənlərin bərabər olub-olmadığını yoxlamaq üçün istifadə olunur. Məsələn, a dəyişəninin dəyəri `5`-ə bərabərdirsə, `true` cavabını göstərəcək:

```javascript
var a = 5;
var b = 5;

console.log(a == b); // true
```

Javascript də tək bərabərlik işarəsi `=` təyin operatorudur. Bərabərlik operatoru isə `==` işarəsidir. Yəni birincisi dəyişənə məlumat mənimsətmək üçün, ikincisi isə dəyişənlərin bərabər olub-olmadığını yoxlamaq üçündür.

2. **Bərabərlikdən fərqli operatoru (!=)**: Dəyişənlərin bərabər olmadığını yoxlamaq üçün istifadə olunur. Məsələn, a dəyişəninin dəyəri `5`-ə bərabər deyilsə, `true` cavabını göstərəcək:

```javascript
var a = 5;
var b = 10;

console.log(a != b); // true
```

3. **Qüsurlu bərabərlik operatoru (===)**: Dəyişənlərin dəyərlərinin və tipinin bərabər olub-olmadığını yoxlamaq üçün istifadə olunur. Məsələn, a dəyişəninin dəyəri `5`-ə bərabər və tipi `number`-ə bərabərdirsə, `true` cavabını göstərəcək:

```javascript
var a = 5;
var b = "5";

console.log(a === b); // false
```

4. **Qüsurlu bərabərlikdən fərqli operatoru (!==)**: Dəyişənlərin dəyərlərinin və tipinin bərabər olmadığını yoxlamaq üçün istifadə olunur. Məsələn, a dəyişəninin dəyəri `5`-ə bərabər və tipi `number`-ə bərabər deyilsə, `true` cavabını göstərəcək:

```javascript
var a = 5;
var b = "5";

console.log(a !== b); // true
```

5. **Kiçikdir operatoru (<)**: Dəyişənlərin kiçik olub-olmadığını yoxlamaq üçün istifadə olunur. Məsələn, a dəyişəninin dəyəri `5`-dən kiçikdirsə, `true` cavabını göstərəcək:

```javascript
var a = 5;
var b = 10;

console.log(a < b); // true
```

6. **Böyükdir operatoru (>)**: Dəyişənlərin böyük olub-olmadığını yoxlamaq üçün istifadə olunur. Məsələn, a dəyişəninin dəyəri `10`-dan böyükdürsə, `true` cavabını göstərəcək:

```javascript
var a = 5;
var b = 10;

console.log(b > a); // true
```

7. **Kiçik bərabərdir operatoru (<=)**: Dəyişənlərin kiçik və ya bərabər olub-olmadığını yoxlamaq üçün istifadə olunur. Məsələn, a dəyişəninin dəyəri `5`-dən kiçik və ya bərabərdirsə, `true` cavabını göstərəcək:

```javascript
var a = 5;
var b = 10;

console.log(a <= b); // true
```

8. **Böyük bərabərdir operatoru (>=)**: Dəyişənlərin böyük və ya bərabər olub-olmadığını yoxlamaq üçün istifadə olunur. Məsələn, a dəyişəninin dəyəri `10`-dan böyük və ya bərabərdirsə, `true` cavabını göstərəcək:

```javascript
var a = 5;
var b = 10;

console.log(b >= a); // true
```

## Javascript məntiqi operatorlar

Js-də məntiqi operatorlar, dəyişənlər arasında məntiqi əməliyyatlar etmək üçün istifadə olunur. Js-də əsas məntiqi operatorlar aşağıdakılardır:

1. **Və operatoru (&&)**: Dəyişənlərin hər ikisi doğru olduğu təqdirdə, `true` cavabını göstərəcək. Məsələn, a və b dəyişənlərinin hər ikisi doğru olduğu təqdirdə, `true` cavabını göstərəcək:

```javascript
var a = true;
var b = true;

console.log(a && b); // true
```

2. **Və ya operatoru (||)**: Dəyişənlərdən biri doğru olduğu təqdirdə, `true` cavabını göstərəcək. Məsələn, a və b dəyişənlərindən biri doğru olduğu təqdirdə, `true` cavabını göstərəcək:

```javascript
var a = true;
var b = false;

console.log(a || b); // true
```

3. **Değil operatoru (!)**: Dəyişənin qarşısındakı dəyəri əks etdirir. Məsələn, a dəyişəninin dəyəri `true` olduğu təqdirdə, `false` cavabını göstərəcək:

```javascript
var a = true;

console.log(!a); // false
```

## Javascript binary (ikili) sistem nədir?

İkili sistem ədədləri 0 və 1 simvolları ilə ifadə edən ədədlər sistemidir. İkili sistem, kompüterlərin əsas ədədlər sistemidir. İkili sistemdə, ədədlər 2 simvoldan istifadə edərək ifadə olunur. Ədədlər 0 və 1 simvolları ilə ifadə olunur. Məsələn ikili sistemdə, 0, 1, 10, 11, 100, 101, 110, 111, 1000, 1001 və s. Bunlar onluq sistemdə 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 ədədlərinə bərabərdir.

Onluq say sistemindəki ədədləri ikili say sistemində ifadə etmək üçün aşağıdakı qayda istifadə olunur:

```
10-luq sistemdəki ədəd / 2 = 2-luq sistemdəki ədəd
```

Məsələn, 10-luq sistemdəki 5 ədədini ikili sistemdə ifadə etmək üçün aşağıdakı qayda istifadə olunur:

```
5 / 2 = 2, qalıq 1
2 / 2 = 1, qalıq 0
1 / 2 = 0, qalıq 1
```

Yuxarıdakı qayda nəticəsində, 10-luq sistemdəki 5 ədədi ikili sistemdə `101` ədədi ilə ifadə olunur.

İkilik sistemdəki ədədləri onluq sistemə çevirmək üçün aşağıdakı qayda istifadə olunur:

```javascript
let binary = 101;
let decimal = parseInt(binary, 2);

console.log(decimal); // 5
```

Burada `parseInt()` funksiyası istifadə olunur. İlk parametr olaraq ikili sistemdəki ədədi, ikinci parametr olaraq isə ikili sistemdəki ədədin növünü göstərir. Əgər ikili sistemdəki ədədləri onluq sistemə çevirmək istəyirsinizsə, ikinci parametr olaraq `2` ədədini göstərməlisiniz. 


# Dərs 1 tapşırıqlar

1. **Javascript-də dəyişənlər arasında riyazi əməliyyatlar etmək**: Riyazi əməliyyatlar etmək üçün dəyişənlər yaradın və riyazi əməliyyatlar yerinə yetirin.
2. **Javascript-də təyin operatorları**: Təyin operatorları ilə dəyişənlərə məlumat mənimsədin.
3. **Javascript-də müqayisə operatorları**: Müqayisə operatorları ilə dəyişənləri müqayisə edin.
4. **Javascript-də məntiqi operatorlar**: Məntiqi operatorlar ilə dəyişənləri müqayisə edin.
5. **Javascript-də ikili sistem**: İkili sistemdəki ədədləri onluq sistemə çevirin. (5, 10, 200, 350, 400)
6. **Javascript-də ikili sistem**: Onluq sistemdəki ədədləri ikili sistemə çevirin. (101, 1001, 1100, 1110, 10000)
7. **Javascript də dataları göstərmək**: Javascript-də `alert()`, `console.log()`, `document.write()`, `innerHTML` metodlarından istifadə edərək, məlumatları göstərin.
8. **Javascript də şərh yazmaq**: Javascript-də şərh yazmaq üçün `//` və ya `/* */` işarələrindən istifadə edin.
9. **Javascript file necə yaradılır**: Javascript fayllarını `.js` uzantılı fayllar ilə yaradın və HTML faylına əlavə edin.
10. **Javascript dəyişənlər**: Javascript-də dəyişənlər yaradın və məlumat mənimsədin.