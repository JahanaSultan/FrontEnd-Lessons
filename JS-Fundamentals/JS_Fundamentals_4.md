# Javascript Dərs 4


## Array Metodları (Array Methods)

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