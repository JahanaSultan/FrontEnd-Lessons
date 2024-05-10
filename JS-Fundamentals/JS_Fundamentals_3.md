# Javascript Dərs 3


##  Number Metodları (Number Methods)

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

4. `parseInt()`: Stringi tam ədədə çevirir.

```javascript
let num = "5";
console.log(parseInt(num)); // 5
```

5. `parseFloat()`: Stringi onluq ədədə çevirir.

```javascript
let num = "5.12345";
console.log(parseFloat(num)); // 5.12345
```

6. `isNaN()`: Numberin `NaN` olub-olmadığını yoxlayır. `NaN` (Not a Number) ədəd olmayan bir dəyəri ifadə edir. Əgər dəyişkən string halında olsa belə ədədə çevrilə bilməyəcək bir dəyərə malikdirsə, `NaN` olaraq qəbul edilir və `isNaN()` funksiyası `true` qaytarır. Əks halda `false` qaytarır. 

```javascript
let num = 5;
console.log(isNaN(num)); // false

num = "5";
console.log(isNaN(num)); // false

num = "Hello";
console.log(isNaN(num)); // true
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


##  Boolean Metodları (Boolean Methods)

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


## Şərt İfadələri (Conditional Statements)

Şərt ifadələri, proqramın müxtəlif şərtlərə uyğun olaraq fərqli əməliyyatlar yerinə yetirməsini təmin edir. JavaScript-də ən çox istifadə olunan şərt ifadələri aşağıdakılardır:

1. `if` şərti: Əgər şərt doğru olarsa, şərtin icra olunacağı blok işlənir.

```javascript
let isStudent = true;

if (isStudent) {
    console.log("You are a student.");
}
```

2. `if...else` şərti: Əgər şərt doğru olarsa, `if` bloku işlənir. Əks halda isə `else` bloku işlənir.

```javascript

let isStudent = false;

if (isStudent) {
    console.log("You are a student.");
} else {
    console.log("You are not a student.");
}
```

3. `if...else if...else` şərti: Əgər bir neçə şərti yoxlamaq lazımdırsa, `if...else if...else` şərti istifadə olunur.

```javascript

let isStudent = false;

if (isStudent) {
    console.log("You are a student.");
} else if (!isStudent) {
    console.log("You are not a student.");
} else {
    console.log("You are not a student.");
}
```

4. `switch` şərti: `switch` şərti, bir neçə eyni dəyəri yoxlamaq üçün istifadə olunur. Bu şərt, `case` blokları ilə təyin olunur. Əgər heç bir `case` bloku doğru olmazsa, `default` bloku işlənir. Bu şərtdən sonra `break` ifadəsi yazılmalıdır. Əks halda, növbəti `case` bloku da işlənəcək. Bu, istifadəçiyə səhv nəticələr göstərə bilər. Çox az hallarda istifadə olunur.

```javascript

let day = "Monday";

switch (day) {
    case "Monday":
        console.log("Today is Monday.");
        break;
    case "Tuesday":
        console.log("Today is Tuesday.");
        break;
    case "Wednesday":
        console.log("Today is Wednesday.");
        break;
    case "Thursday":
        console.log("Today is Thursday.");
        break;
    case "Friday":
        console.log("Today is Friday.");
        break;
    case "Saturday":
        console.log("Today is Saturday.");
        break;
    case "Sunday":
        console.log("Today is Sunday.");
        break;
    default:
        console.log("Invalid day.");
}
```

5. Ternary operatorları, `if...else` şərt ifadələrinin qısa formalarıdır. Ternary operatorları, üç əsas hissədən ibarətdir: şərt, şərtin doğru olması halında icra olunacaq əməliyyat və şərtin yanlış olması halında icra olunacaq əməliyyat. Ternary operatorları aşağıdakı kimi yazılır:

```javascript

let isStudent = true;

let message = isStudent ? "You are a student." : "You are not a student.";

console.log(message);
```

və ya sadəcə `true` halında icra olunması gərəkən və `else` şərti olmadan:

```javascript

let isStudent = true;

isStudent && console.log("You are a student.");
```

6. `nullish coalescing` operatoru: `nullish coalescing` operatoru, `null` və ya `undefined` dəyərlərini yoxlamaq üçün istifadə olunur. Əgər dəyişkən `null` və ya `undefined` dəyərindən başqa bir dəyərə malikdirsə, bu dəyəri qaytarır. Əks halda, ikinci dəyəri qaytarır.

```javascript

let name = "John";
let message = name ?? "Guest";

console.log(message); // "John"
```


##  Dövr Operatorları (Loop Statements)

Dövr operatorları, müxtəlif şərtlərə uyğun olaraq eyni əməliyyatı təkrar təkrar yerinə yetirmək üçün istifadə olunur. Javascriptdə kodlar normalda yuxarıdan aşağı işlənir. Dövr operatorları, kodun müəyyən bir hissəsini təkrar təkrar işlədərək proqramın nəzərdə tutulan məqsədə çatmasını təmin edir. JavaScript-də ən çox istifadə olunan dövr operatorları aşağıdakılardır:

1. `for` dövrü: `for` dövrü, müəyyən bir şərtə uyğun olaraq bir bloku təkrar təkrar işləmək üçün istifadə olunur.

```javascript

for (let i = 0; i < 5; i++) {
    console.log(i);
}
```

2. `while` dövrü: `while` dövrü, bir şərt doğru olduğu müddətdə bir bloku təkrar təkrar işləmək üçün istifadə olunur.

```javascript

let i = 0;

while (i < 5) {
    console.log(i);
    i++;
}
```

3. `do-while`: `do-while` dövr operatoru, ən az bir dəfə icra olunacaq əməliyyatları icra etmək üçün istifadə olunur. Dövrün icra edilip edilmədiyi, dövrün sonunda şərtin doğru olub olmamasına əsaslanır.Məsələn:

```javascript

let i = 0;

do {
    console.log(i);
    i++;
} while (i < 5);
```

`break` və `continue` ifadələri:

1. `break` ifadəsi: `break` ifadəsi, dövrü dayandırmaq üçün istifadə olunur.

```javascript

for (let i = 0; i < 5; i++) {
    if (i === 3) {
        break;
    }
    console.log(i);
} // 0, 1, 2
```

2. `continue` ifadəsi: `continue` ifadəsi, dövrün növbəti addımına keçmək üçün istifadə olunur.

```javascript

for (let i = 0; i < 5; i++) {
    if (i === 3) {
        continue;
    }
    console.log(i);
}// 0, 1, 2, 4
```


# Dərs 3 Tapşırıqlar

1. Ədədin mənfi və ya müsbət olduğunu yoxlayan proqram yazın.
2. İstifadəçinin yaşına görə, istifadəçinin yaşının 18-dən böyük olub-olmadığını yoxlayan proqram yazın.
3. İstifadəçinin yaşına görə, istifadəçinin yaşının 18-dən böyük olduğu halda, istifadəçinin sürücülük vəsiqəsinin olub-olmadığını yoxlayan proqram yazın.
4. Ədədin cüt və ya tək olduğunu yoxlayan proqram yazın.
5. FizzBuzz oyunu yazın. (Əgər ədəd 3-ə və 5-ə bölünürsə, "FizzBuzz" çap edin. Əgər ədəd 3-ə bölünürsə, "Fizz" çap edin. Əgər ədəd 5-ə bölünürsə, "Buzz" çap edin. Əks halda, ədədi çap edin.)
6. İstifadəçinin daxil etdiyi ədədin faktorialını hesablayan proqram yazın. (prompt() funksiyası ilə istifadəçidən məlumat alın.)
7. İstifadəçinin daxil etdiyi iki ədədin ƏBOB və ƏKOB-nu hesablayan proqram yazın. (prompt() funksiyası ilə istifadəçidən məlumat alın.)
8. İstifadəçinin daxil etdiyi iki ədəd arasındakı ədədlərdən cüt olanları çap edən proqram yazın. (prompt() funksiyası ilə istifadəçidən məlumat alın.)
9. İstifadəçinin daxil etdiyi cümlədə müəyyən bir sözün olub-olmadığını yoxlayan proqram yazın. (prompt() funksiyası ilə istifadəçidən məlumat alın.)
10. İstifadəçinin daxil etdiyi cümlədəki sözlərin sayını hesablayan proqram yazın. (prompt() funksiyası ilə istifadəçidən məlumat alın.)
11. İstifadəçinin daxil etdiyi cümlədəki hərflərin sayını hesablayan proqram yazın. (prompt() funksiyası ilə istifadəçidən məlumat alın.)
12. İstifadəçidən password yazmasını tələb edin və password-da ən azı bir böyük hərf, bir kiçik hərf, bir rəqəm və bir simvol olub-olmadığını yoxlayan proqram yazın. Əgər bu şərtlər ödənmirsə yeni bir şifrə yazması üçün program nəyin əksik olduğunu bildirib yenidən şifrə yazmağı tələb etsin. Əks halda 
"Şifrə qəbul edildi yazılsın" (prompt() funksiyası ilə istifadəçidən məlumat alın.)
13. İstifadəçinin daxil etdiyi ədədin rəqəmlərinin cəmini hesablayan proqram yazın. (prompt() funksiyası ilə istifadəçidən məlumat alın.)
14. İstifadəçinin daxil etdiyi ədədin rəqəmlərinin hasilini hesablayan proqram yazın. (prompt() funksiyası ilə istifadəçidən məlumat alın.)
15. Prompt dan daxil edilmiş tələbənin qiymətini yoxlayın. 90 və yuxarı olarsa "A", 80 və yuxarı olarsa "B", 70 və yuxarı olarsa "C", 60 və yuxarı olarsa "D", əks halda "F" yazın. (prompt() funksiyası ilə istifadəçidən məlumat alın.)
16. Bilet qiymətini daxil edən istifadəçidən yaşını daxil etməsini tələb edin. Əgər yaş 65-dən böyük və ya 12-dən kiçikdirsə, biletin qiyməti 7 dollar olmalıdır. Əks halda biletin qiyməti 12 dollar olmalıdır. Biletin qiymətini çap edin. (prompt() funksiyası ilə istifadəçidən məlumat alın.)
17. Məhsulun qiymətinə görə tətbiq olanan endirim faizini hesablayan proqram yazın. Əgər məhsulun qiyməti 1000 dollar və yuxarıdırsa, endirim faizi 10% olmalıdır. Əks halda endirim faizi 5% olmalıdır. Endirim faizini və endirimli qiyməti çap edin. (prompt() funksiyası ilə istifadəçidən məlumat alın.)
18. Bədən çəki indeksini hesablayan proqram yazın. İstifadəçidən çəkisini və boyunu soruş. Hesablanma qaydası: çəki / boy**2 (boy 160 çəki 60 dırsa 60 / 1.6 * 1.6)  Bədən çəki indeksi 18.5-dən kiçikdirsə, "Aşağıdır", 18.5-dən böyükdür və 24.9-dan kiçikdirsə, "Normaldır", 24.9-dan böyükdür və 29.9-dan kiçikdirsə, "Çox çoxdur", 29.9-dan böyükdürsə, "Obezdir" yazın. (prompt() funksiyası ilə istifadəçidən məlumat alın.)