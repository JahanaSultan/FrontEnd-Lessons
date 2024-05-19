# Javascript Dərs 5

## Obyektlər(Objects)

Obyektlər, əlaqəli məlumatları bir yerdə saxlamaq üçün ideal bir yoldur. Bu, məlumatların daha strukturlaşdırılmış və məntiqi bir şəkildə təşkil edilməsinə kömək edir. Məsələn, bir istifadəçi haqqında məlumatları saxlamaq istəyirsinizsə, ayrı-ayrı dəyişənlərdən istifadə etmək əvəzinə, bir obyekt istifadə edə bilərsiniz:


```javascript
let user = {
  name: "John",
  age: 30,
  isAdmin: true,
};
```

Boş array yaratmaq üçün iki, yəni köhnə və yeni sintaksis var:

```javascript
let user = new Object(); // "object constructor" syntax
let user = {};  // "object literal" syntax
```

Obyektin daxilindəki məlumatlara "property" deyilir. "key: value" formatında yazılır. Məsələn, burada `name`, `age` və `isAdmin` property-ləridir.

Property-lərə daxil olmaq üçün iki üsul var:

```javascript
console.log( user.name ); // John
console.log( user.age ); // 30
```

Property-ləri dəyişdirmək və ya silmək üçün aşağıdakı metodlardan istifadə edə bilərik:

```javascript
user.isAdmin = false; // property-ni dəyişdik
delete user.age; // property-ni silərik
```

Obyektin içindəki property-ləri öyrənmək üçün `Object.keys` istifadə edə bilərsiniz. Bu metod bizə objectin `key` lərini array şəklində geri qaytarır:

```javascript
let user = {
  name: "John",
  age: 30,
  isAdmin: true
};

console.log(Object.keys(user) ); // ["name", "age", "isAdmin"]
```

Eyni şəkildə value ləri array şəklində əldə etmək üçün `Objects.values()` metodundan istifadə edə bilərik. Bu bizə obyektin valuelərini array şəklində geri qatrarır:

```javascript
let user = {
  name: "John",
  age: 30,
  isAdmin: true
};

console.log(Object.values(user) ); // ["John", 30, true]
```

Obyektin içindəki key və valueləri array içində array şəklinə çevirmək üçün `Object.entries()` metodundan istifadə olunur:

```javascript
let user = {
  name: "John",
  age: 30,
  isAdmin: true
};

console.log(Object.entries(user) ); // [["name","John"], ["age",30], ["isAdmin",true]]
```

Obyektin içindəki bütün property-lərə daxil olmaq üçün `for..in` dövr operatorunu istifadə edə bilərsiniz:

```javascript
let user = {
  name: "John",
  age: 30,
  isAdmin: true
};

for (let key in user) {
  cobnsole.log( key ); // name, age, isAdmin
  cobnsole.log( user[key] ); // John, 30, true
}
```

## Obyektlərin metodları

Obyektin içindəki property-lərə əlavə olaraq, obyektin içində metodlar da saxlaya bilərik. Məsələn, aşağıdakı obyektin içində `fullName` adlı metod var:

```javascript
let user = {
  name: "John",
  surname: "Doe",
  age: 30,
  isAdmin: true,
  fullName: function() {
    return this.name + " " + this.surname;
  }
};

console.log( user.fullName() ); // John Doe
```

Yuxarıdakı metodun digər bir yazılış üsulu da var:

```javascript
let user = {
  name: "John",
  surname: "Doe",
  age: 30,
  isAdmin: true,
  fullName() {
    return this.name + " " + this.surname;
  }
};

console.log( user.fullName() ); // John Doe
```

## Obyektin içində this

`this` obyektin özünü göstərir. Məsələn, aşağıdakı kodda `this` obyekti göstərir:

```javascript
let user = {
  name: "John",
  surname: "Doe",
  age: 30,
  isAdmin: true,
  fullName() {
    return this.name + " " + this.surname;
  }
};

console.log( user.fullName() ); // John Doe
```

## Obyektin içində yeni property əlavə etmək

Obyektin içində yeni property əlavə etmək üçün aşağıdakı sintaksisi istifadə edə bilərsiniz:

```javascript
let user = {
  name: "John",
  surname: "Doe",
  age: 30,
  isAdmin: true,
};

user.newProperty = "new value";
```

## Obyektin içində yeni metod əlavə etmək

Obyektin içində yeni metod əlavə etmək üçün aşağıdakı sintaksisi istifadə edə bilərsiniz:

```javascript
let user = {
  name: "John",
  surname: "Doe",
  age: 30,
  isAdmin: true,
  fullName() {
    return this.name + " " + this.surname;
  }
};

user.newMethod = function() {
  return "Hello";
};

console.log( user.newMethod() ); // Hello
```

## Obyektin içində property-ləri silmək

Obyektin içində property-ləri silmək üçün `delete` operatorundan istifadə edə bilərsiniz:

```javascript
let user = {
  name: "John",
  surname: "Doe",
  age: 30,
  isAdmin: true,
};

delete user.age;
```

## Obyektin içində property-ləri yoxlamaq

Obyektin içində property-ləri yoxlamaq üçün `in` operatorundan istifadə edə bilərsiniz:

```javascript
let user = {
  name: "John",
  surname: "Doe",
  age: 30,
  isAdmin: true,
};

console.log( "name" in user ); // true

console.log( "age" in user ); // false
```

## Math obyekti

`Math` obyekti, riyazi əməliyyatlar üçün metodlar təklif edir.

`Math.random()` metodu 0 ilə 1 arasında təsadüfi bir rəqəm qaytarır:

```javascript
console.log( Math.random() ); // təsadüfi bir rəqəm
```

`Math.ceil()` metodu, verilmiş rəqəmi yuxarıya doğru yuvarlaqlaşdırır:

```javascript

console.log( Math.ceil(1.1) ); // 2
```

`Math.floor()` metodu, verilmiş rəqəmi aşağıya doğru yuvarlaqlaşdırır:

```javascript

console.log( Math.floor(1.9) ); // 1
```

`Math.round()` metodu, verilmiş rəqəmi yaxınlıq prinsipinə əsasən yuvarlaqlaşdırır:

```javascript

console.log( Math.round(1.4) ); // 1
console.log( Math.round(1.5) ); // 2
```

`Math.max()` metodu, verilmiş rəqəmlərin ən böyüyünü qaytarır:

```javascript

console.log( Math.max(1, 2, 3) ); // 3
```

`Math.min()` metodu, verilmiş rəqəmlərin ən kiçiyini qaytarır:

```javascript

console.log( Math.min(1, 2, 3) ); // 1
```

`Math.pow()` metodu, verilmiş rəqəmin verilmiş qüvvətini qaytarır:

```javascript

console.log( Math.pow(2, 3) ); // 8
```

`Math.sqrt()` metodu, verilmiş rəqəmin kvadrat kökünü qaytarır:

```javascript

console.log( Math.sqrt(9) ); // 3
```

`Math.abs()` metodu, verilmiş rəqəmin modulunu qaytarır:

```javascript

console.log( Math.abs(-3) ); // 3
```

## Date obyekti

`Date` obyekti, tarix və saat məlumatlarını saxlamaq üçün istifadə olunur. Məsələn, aşağıdakı kodda, `Date` obyekti yaradılır və tarix və saat məlumatları göstərilir:

```javascript
let date = new Date();

console.log( date ); // Sat May 01 2021 15:45:12 GMT+0400 (Azerbaijan Standard Time)
```

`Date` obyektinin dəyişənləri aşağıdakı kimi olur:

- `getFullYear()` - il
- `getMonth()` - ay
- `getDate()` - gün
- `getHours()` - saat
- `getMinutes()` - dəqiqə
- `getSeconds()` - saniyə
- `getMilliseconds()` - millisaniyə
- `getDay()` - həftənin günü

Məsələn, aşağıdakı kodda, `Date` obyektinin dəyişənlərindən istifadə olunur:

```javascript
let date = new Date();

console.log( date.getFullYear() ); // 2021
console.log( date.getMonth() ); // 4
console.log( date.getDate() ); // 1
console.log( date.getHours() ); // 15
console.log( date.getMinutes() ); // 45
console.log( date.getSeconds() ); // 12
console.log( date.getMilliseconds() ); // 0
console.log( date.getDay() ); // 6
```

## Date obyektinin metodları

`Date` obyektinin metodlarından biri `setFullYear()` metodudur. Bu metod, ilin dəyişdirilməsini təmin edir:

```javascript

let date = new Date();

date.setFullYear(2022);

console.log( date.getFullYear() ); // 2022
```

`setMonth()` metodu, ayın dəyişdirilməsini təmin edir:

```javascript

let date = new Date();

date.setMonth(5);

console.log( date.getMonth() ); // 5
```

`setDate()` metodu, günün dəyişdirilməsini təmin edir:

```javascript

let date = new Date();

date.setDate(2);

console.log( date.getDate() ); // 2
```

`setHours()` metodu, saatin dəyişdirilməsini təmin edir:

```javascript

let date = new Date();

date.setHours(16);

console.log( date.getHours() ); // 16
```

`setMinutes()` metodu, dəqiqənin dəyişdirilməsini təmin edir:

```javascript

let date = new Date();

date.setMinutes(50);


console.log( date.getMinutes() ); // 50
```

`setSeconds()` metodu, saniyənin dəyişdirilməsini təmin edir:

```javascript

let date = new Date();

date.setSeconds(20);

console.log( date.getSeconds() ); // 20
```

`setMilliseconds()` metodu, millisaniyənin dəyişdirilməsini təmin edir:

```javascript

let date = new Date();

date.setMilliseconds(100);

console.log( date.getMilliseconds() ); // 100
```

`setDay()` metodu, həftənin gününün dəyişdirilməsini təmin edir:

```javascript

let date = new Date();

date.setDay(0);

console.log( date.getDay() ); // 0
```

## Date obyektinin formatlandırılması

`Date` obyektinin formatlandırılması üçün aşağıdakı kod nümunəsində olduğu kimi `toLocaleString()` metodu istifadə olunur:

```javascript

let date = new Date();

console.log( date.toLocaleString() ); // 5/1/2021, 3:45:12 PM
```

## Date obyektinin tarix və saat məlumatlarının əldə edilməsi

`Date` obyektinin tarix və saat məlumatlarını əldə etmək üçün aşağıdakı kod nümunəsində olduğu kimi `toDateString()` və `toTimeString()` metodları istifadə olunur:

```javascript

let date = new Date();

console.log( date.toDateString() ); // Sat May 01 2021

console.log( date.toTimeString() ); // 15:45:12 GMT+0400 (Azerbaijan Standard Time)
```
# Dərs 5 Tapşırıqlar

1. İstifadəçilərdən ibarət object yaradın. Ən azı 5 istifadəçinin məlumatlarını ehtiva etsin və aşağıdakı əməliyyatları həmin object üzərində aparın:

- İstifadəçilərin sayını ekrana çap edin
- İstifadəçilərin adlarını ekrana çap edin
- İstifadəçilərin yaşlarını ekrana çap edin
- Bu object içində yaşı ən böyük olan və ən kiçik olan istifadəçini consola çıxarın.
- İstifadəçilərin yaşlarının cəmini ekrana çap edin
- İstifadəçilərin yaşlarının ortalamasını ekrana çap edin

2. Aşağıdakı obyektlər üzərində qeyd olunan əməliyyarları icra edin:

```javascript
let students = [
  {
    name : "Fəridə Qafarova",
    age : 20,
    group : "P501",
    grades : [90, 80, 70, 60],
    lessons: ["Math", "Physics", "Chemistry", "Biology"]
  },
  {
    name : "Nərmin Quliyeva",
    age : 21,
    group : "P502",
    grades : [80, 70, 60, 50],
    lessons: ["Literature", "Physics", "Chemistry", "Music"]
  },
  {
    name : "Nəzrin Quliyeva",
    age : 22,
    group : "P503",
    grades : [70, 60, 50, 40],
    lessons: ["Economics", "Physics", "Chinese", "Biology"]
  },
  {
    name : "Nərmin Qafarova",
    age : 23,
    group : "P504",
    grades : [60, 50, 40, 30],
    lessons: ["Math", "Physics", "History", "Biology"]
  },
  {
    name : "Fəridə Quliyeva",
    age : 24,
    group : "P505",
    grades : [50, 40, 30, 20],
    lessons: ["Math", "Art", "Drama", "Geography"]
  }
]
```

- Tələbələrin qiymət ortalamalarını ekrana çıxarın.(Filankesov Filankes - 45.3)
- Ortalaması sadəcə 50 dən yuxarı olanları ekrana çıxarın.
- Math dərsi alanları ekrana çıxarın.
- Ortalaması ən yüksək olan tələbəni ekrana çıxarın.
- Ortalaması ən aşağı olan tələbəni ekrana çıxarın.
- Sırası ilə hansı dərsdən hansı qiyməti aldığını ekrana çıxarın.(Qiymətlər və dərslər obyektdə eyni sıra ilə düzülüb)
- Chemistry dərsi alanların qiymət ortalamalarını ekrana çap edin.
- Bütün tələbələrin aldığı bütün dərsləri unik şəkildə ekrana array şəklində çap edin.

3. Promptdan rəqəmlə daxil edilmiş ədədi consolda hərflə çap edin.

```javascript

let propmt = 523
console.log(prompt) // beş yüz iyirmi üç
```

4. Ölkələr, paytaxtları, rəsmi dillərini ehtiva edən obyektlər yaradın və promptdan daxil edilən ölkəni tapıb silin.
  
  ```javascript
  let countries = [
    {
      name: "Azerbaijan",
      capital: "Baku",
      language: "Azerbaijani"
    },
    {
      name: "Turkey",
      capital: "Ankara",
      language: "Turkish"
    },
    {
      name: "Russia",
      capital: "Moscow",
      language: "Russian"
    },
    {
      name: "Germany",
      capital: "Berlin",
      language: "German"
    },
    {
      name: "France",
      capital: "Paris",
      language: "French"
    }
  ]

  let country = prompt("Ölkə adını daxil edin")
  ```

5. Math obyektindən istifadə edərək aşağıdakı əməliyyatları həyata keçirin:

- Ən böyük rəqəmi ekrana çap edin
- Ən kiçik rəqəmi ekrana çap edin
- Ən yaxın tam rəqəmi ekrana çap edin
- 5.6 rəqəminin üstənə yuvarlaqlaşdırın
- 5.6 rəqəminin aşağısına yuvarlaqlaşdırın
- 5.6 rəqəminin kvadrat kökünü ekrana çap edin
- 5.6 rəqəminin modulunu ekrana çap edin
- 5.6 rəqəminin 7-ci dərəcəsinə yüksəldin
- 5.6 və 7.8 rəqəmlərinin ən böyük ortaq bölənini ekrana çap edin
- 5.6 və 7.8 rəqəmlərinin ən kiçik ortaq bölənini ekrana çap edin

6. Date obyektindən istifadə edərək aşağıdakı əməliyyatları həyata keçirin:

- İl, ay, gün, saat, dəqiqə, saniyə, millisaniyə və həftənin gününü ekrana çap edin
- Tarixi formatlandırın
- Tarix və saat məlumatlarını ayrı-ayrı ekrana çap edin
- Cari tarixi ekrana çap edin
- Cari tarixdən 1 gün əvvəl olan tarixi ekrana çap edin
- Cari tarixdən 1 gün sonra olan tarixi ekrana çap edin
- Cari tarixdən 1 ay əvvəl olan tarixi ekrana çap edin
- Cari tarixdən 1 ay sonra olan tarixi ekrana çap edin
- Cari tarixdən 1 il əvvəl olan tarixi ekrana çap edin

7. Tarix məlumatlarını Azərbaycan dilində çap edin.