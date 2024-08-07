# CSS Dərs 8

## Media query

Media query, CSS-in responsive dizayn üçün istifadə olunan bir alətdir. Media query vasitəsilə ekran ölçüsünə uyğun olaraq CSS qaydası təyin edilir.

Media query, CSS-in `@media` rəhbərliyi ilə təyin olunur. Mobil və ya tablet ekranlar üçün fərqli dizayn təyin etmək üçün media query-də `max-width` və `min-width` xüsusiyyətləri istifadə olunur.

```css

/* 600 pikseldən kiçik ekranlar üçün */
@media only screen and (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}

/* 600 pikseldən böyük ekranlar üçün */

@media only screen and (min-width: 600px) {
  body {
    background-color: lightgreen;
  }
}

```

Yuxarıdakı nümunədə `max-width` və `min-width` xüsusiyyətləri ilə ekran ölçüsünə uyğun olaraq CSS qaydası təyin olunur.

Media query-də istifadə olunan xüsusiyyətlər:

- `max-width`: Maksimum ekran ölçüsü
- `min-width`: Minimum ekran ölçüsü
- `max-height`: Maksimum ekran hündürlüyü
- `min-height`: Minimum ekran hündürlüyü

Media query-də istifadə olunan nümunələr:

- `only screen`: Yalnız ekranlar üçün
- `only print`: Yalnız çap üçün
- `only speech`: Yalnız səsli oxuma üçün


## Media query nümunəsi

```css
/* 600 pikseldən kiçik ekranlar üçün */

@media only screen and (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}

/* 600 pikseldən böyük ekranlar üçün */

@media only screen and (min-width: 600px) {
  body {
    background-color: lightgreen;
  }
}
```