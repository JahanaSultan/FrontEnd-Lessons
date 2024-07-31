# CSS Dərs 7


## CSS pseudo-class-lar

CSS pseudo-class-lar, HTML elementlərinin spesifik durumlarını seçmək üçün istifadə olunan seçicilərdir. Pseudo-class-lar, elementlərə dinamik olaraq class əlavə etmək imkanı verir.

Pseudo-class-lar, `:` işarəsi ilə işarələnir və elementin durumuna görə seçim edilir.

Pseudo-class-ların nümunələri:

- `:hover` - Elementə mouse ilə hover edildikdə
- `:active` - Elementə click edildikdə
- `:focus` - Elementə focus olunduqda
- `:first-child` - Elementin ilk child-ı olduğu zaman
- `:last-child` - Elementin son child-ı olduğu zaman
- `:nth-child()` - Elementin n-ci child-ı olduğu zaman
- `:nth-last-child()` - Elementin sonuncu n-ci child-ı olduğu zaman
- `:nth-of-type()` - Elementin n-ci tip child-ı olduğu zaman
- `:nth-last-of-type()` - Elementin sonuncu n-ci tip child-ı olduğu zaman
- `:not()` - Elementin seçilməməsi üçün
- `:checked` - Checkbox və radio button-ların seçilmiş olduğu zaman
- `:disabled` - Elementin disabled olduğu zaman
- `:enabled` - Elementin enabled olduğu zaman
- `:empty` - Elementin boş olduğu zaman
- `:target` - URL-dəki anchor linklərə click edildikdə
- `:root` - Document-in root elementi olduğu zaman
- `:lang()` - Elementin dilinə görə seçim edilməsi üçün
- `:first-of-type` - Elementin ilk tip child-ı olduğu zaman
- `:last-of-type` - Elementin son tip child-ı olduğu zaman
- `:only-of-type` - Elementin yeganə tip child-ı olduğu zaman
- `:only-child` - Elementin yeganə child-ı olduğu zaman
- `:visited` - Linkin ziyarət edildiyi zaman
- `:required` - Elementin required olduğu zaman
- `:optional` - Elementin optional olduğu zaman
- `:valid` - Elementin valid olduğu zaman
- `:invalid` - Elementin invalid olduğu zaman
- `:in-range` - Elementin min və max aralığında olduğu zaman
- `:out-of-range` - Elementin min və max aralığında olmadığı zaman
- `:read-only` - Elementin read-only olduğu zaman
- `:read-write` - Elementin read-write olduğu zaman
- `:default` - Elementin default olduğu zaman
- `:indeterminate` - Checkbox və radio button-ların indeterminate olduğu zaman
- `:nth-match()` - Elementin n-ci child-ı olduğu zaman
- `:nth-last-match()` - Elementin sonuncu n-ci child-ı olduğu zaman
- `:any-link` - Linkin bir link olduğu zaman
- `:local-link` - Linkin eyni domaində olduğu zaman
- `:scope` - Elementin scope olduğu zaman
- `:current` - Linkin current olduğu zaman
- `:past` - Elementin past olduğu zaman
- `:future` - Elementin future olduğu zaman
- `:active-drop-target` - Elementin active drop target olduğu zaman
- `:valid-drop-target` - Elementin valid drop target olduğu zaman
- `:is()` - Elementin seçilməsi üçün
- `:where()` - Elementin seçilməsi üçün
- `:has()` - Elementin seçilməsi üçün

Nümunə:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dərs 7</title>
    <style>
        a {
            color: blue;
        }

        a:hover {
            color: red;
        }

        a:active {
            color: green;
        }

        a:visited {
            color: purple;
        }
    </style>
</head>
<body>
    <a href="#">Link</a>
</body>
</html>
```

Yuxarıdakı nümunədə, `a` elementinə mouse ilə hover edildikdə, click edildikdə, ziyarət edildikdə və normal halda rəngi dəyişir.

CSS pseudo-class-ların daha çox nümunələri üçün [bu ünvanı](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes) ziyarət edə bilərsiniz.


## CSS pseudo-element-lər

CSS pseudo-element-lər, HTML elementlərinin spesifik hissələrini seçmək üçün istifadə olunan seçicilərdir. Pseudo-element-lər, elementlərin içindəki spesifik hissələri seçmək üçün istifadə olunur.

Pseudo-element-lər, `::` işarəsi ilə işarələnir və elementin spesifik hissəsinə görə seçim edilir.

Pseudo-element-lərin nümunələri:

- `::first-line` - Elementin ilk sətrinə görə seçim edilməsi üçün
- `::first-letter` - Elementin ilk hərfinə görə seçim edilməsi üçün
- `::before` - Elementin içindən əvvəl hissə əlavə etmək üçün
- `::after` - Elementin içindən sonra hissə əlavə etmək üçün
- `::selection` - Elementin seçilmiş hissəsinə görə seçim edilməsi üçün
- `::placeholder` - Elementin placeholder hissəsinə görə seçim edilməsi üçün
- `::marker` - List elementlərin marker hissəsinə görə seçim edilməsi üçün

Nümunə:

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dərs 7</title>
    <style>
        p::first-line {
            color: red;
        }

        p::first-letter {
            font-size: 30px;
        }

        p::before {
            content: "Əvvəl: ";
        }

        p::after {
            content: " Sonra";
        }

        p::selection {
            background-color: yellow;
        }
    </style>
</head>
<body>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed ac
        ultricies nunc. Nullam nec nisl nec nisl tincidunt ultricies. 
        Donec auctor, nunc nec ultricies ultricies, nunc nisl tincidunt 
        ultricies. Donec auctor, nunc nec ultricies ultricies, nunc nisl 
        tincidunt ultricies.</p>
</body>
</html>
```

Yuxarıdakı nümunədə, `p` elementinin ilk sətri qırmızı rəngdə, ilk hərfi 30px ölçüsündə, içindən əvvəl "Əvvəl: " və sonra " Sonra" hissələri əlavə olunur, seçilmiş hissə isə sarı rəngdə göstərilir.

CSS pseudo-element-lərin daha çox nümunələri üçün [bu ünvanı](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-elements) ziyarət edə bilərsiniz.


## CSS !important

CSS `!important` ifadəsi, CSS deklarasiyalarında prioriteti artırmaq üçün istifadə olunan ifadədir. Məsələn, bir CSS deklarasiyası normal olaraq işləmir və ya başqa bir CSS deklarasiyası tərəfindən override olunur və ya bir CSS deklarasiyası digər CSS deklarasiyasından daha yüksək prioritetdə olmalıdır.

`!important` ifadəsi, CSS deklarasiyasının sonuna əlavə olunur.

Nümunə:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dərs 7</title>
    <style>
        p {
            color: red !important;
        }

        p {
            color: blue;
        }
    </style>
</head>

<body>
    <p>Text</p>
</body>
</html>
```

Yuxarıdakı nümunədə, `p` elementinə qırmızı rəng təyin edilir. CSS deklarasiyasının sonunda `!important` ifadəsi olduğu üçün, digər CSS deklarasiyası işləməz və `p` elementi qırmızı rəngdə göstərilir.

`!important` ifadəsindən istifadə etmək CSS-in oxunuluşunu çətinləşdirə bilər. Bu səbəbdə, `!important` ifadəsindən istifadə etməkdən çəkinmək daha məqsədəuyğundur.


## CSS Math Functions

CSS Math Functions, CSS-də hesablama apara bilmək üçün istifadə olunan funksiyalardır.

CSS Math Functions nümunələri:

- `calc()` - CSS-in hesablama funksiyasıdır. `calc()` funksiyası, CSS-in hesablama funksiyalarını birlikdə istifadə etməyə imkan verir.
- `min()` - CSS-in minimum funksiyasıdır. `min()` funksiyası, CSS-in minimum funimallarını birlikdə istifadə etməyə imkan verir.
- `max()` - CSS-in maksimum funksiyasıdır. `max()` funksiyası, CSS-in maksimum funimallarını birlikdə istifadə etməyə imkan verir.

Nümunə:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dərs 7</title>
    <style>
        div {
            width: calc(100% - 100px);
            height: 100px;
            background-color: red;
        }

        p {
            width: min(100%, 200px);
            height: 100px;
            background-color: blue;
        }

        span {
            width: max(100%, 200px);
            height: 100px;
            background-color: green;
        }
    </style>
</head>
<body>
    <div></div>
    <p></p>
    <span></span>
</body>
</html>
```

Yuxarıdakı nümunədə, `div` elementinə `calc()` funksiyası ilə genişlik təyin edilir. `p` elementinə `min()` funksiyası ilə genişlik təyin edilir. `span` elementinə `max()` funksiyası ilə genişlik təyin edilir.


## CSS `:root` Selector

CSS `:root` selector, HTML sənədinin root elementini seçmək üçün istifadə olunan seçicidir. Root element, HTML sənədinin ən üst elementidir.

`:root` selector, `html` elementinə bərabərdir.

Nümunə:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dərs 7</title>
    <style>
        :root {
            --color: red;
        }

        p {
            color: var(--color);
        }
    </style>

</head>

<body>
    <p>Text</p>

</body>
</html>
```

Yuxarıdakı nümunədə, `:root` selector ilə `--color` adlı CSS custom property təyin edilir. `p` elementinə `var()` funksiyası ilə `--color` adlı CSS custom property təyin edilir.

`:root` selector, CSS custom property-lər təyin etmək üçün istifadə olunur.


## CSS `@import` Rule

CSS `@import` rule, CSS fayllarını başqa CSS fayllarına import etmək üçün istifadə olunan qayda.

`@import` rule, CSS fayllarını import etmək üçün istifadə olunur. CSS fayllarını import etmək üçün, `@import` rule-dan sonra import ediləcək CSS faylının ünvanı yazılır.

Nümunə:

```css
@import url("style.css");
```

Yuxarıdakı nümunədə, `style.css` faylı import edilir.


## CSS 2D Transforms

Css 2D Transforms, elementləri 2D düzəndə dəyişdirmək üçün istifadə olunan CSS xüsusiyyətləridir. 

Aşağıdakı 2D Transforms xüsusiyyətləri mövcuddur:

- `translate()` - Elementi x və y istiqamətində dəyişdirmək üçün istifadə olunur.
- `rotate()` - Elementi döndərmək üçün istifadə olunur.
- `scale()` - Elementi ölçüdə dəyişdirmək üçün istifadə olunur.
- `skew()` - Elementi x və y istiqamətində dəyişdirmək üçün istifadə olunur.
- `matrix()` - Elementi 2D matrix transformasiyası ilə dəyişdirmək üçün istifadə olunur.

Nümunə:

```css
div {
    transform: translate(50px, 100px);
    transform: rotate(45deg);
    transform: scale(2, 2);
    transform: skew(30deg, 20deg);
    transform: matrix(1, 0.5, -0.5, 1, 30, 10);
}
```

Yuxarıdakı nümunədə, `div` elementinə `transform` xüsusiyyəti ilə element dəyişdirilir.


## CSS 3D Transforms

Css 3D Transforms, elementləri 3D düzəndə dəyişdirmək üçün istifadə olunan CSS xüsusiyyətləridir.

Aşağıdakı 3D Transforms xüsusiyyətləri mövcuddur:

- `rotateX()` - Elementi x oxuna görə döndərmək üçün istifadə olunur.
- `rotateY()` - Elementi y oxuna görə döndərmək üçün istifadə olunur.
- `rotateZ()` - Elementi z oxuna görə döndərmək üçün istifadə olunur.
- `rotate3d()` - Elementi 3D oxuna görə döndərmək üçün istifadə olunur.
- `scaleX()` - Elementi x oxunda ölçüdə dəyişdirmək üçün istifadə olunur.
- `scaleY()` - Elementi y oxunda ölçüdə dəyişdirmək üçün istifadə olunur.
- `scaleZ()` - Elementi z oxunda ölçüdə dəyişdirmək üçün istifadə olunur.
- `scale3d()` - Elementi 3D oxunda ölçüdə dəyişdirmək üçün istifadə olunur.
- `translateX()` - Elementi x oxunda dəyişdirmək üçün istifadə olunur.
- `translateY()` - Elementi y oxunda dəyişdirmək üçün istifadə olunur.

Nümunə:

```css
div {
    transform: rotateX(45deg);
    transform: rotateY(45deg);
    transform: rotateZ(45deg);
    transform: rotate3d(1, 1, 1, 45deg);
    transform: scaleX(2);
    transform: scaleY(2);
    transform: scaleZ(2);
    transform: scale3d(2, 2, 2);
    transform: translateX(50px);
    transform: translateY(50px);
}
```

Yuxarıdakı nümunədə, `div` elementinə `transform` xüsusiyyəti ilə element 3D düzəndə dəyişdirilir.


## CSS Animations

CSS Animations, elementlərə animasiya əlavə etmək üçün istifadə olunan CSS xüsusiyyətləridir.

CSS Animations xüsusiyyətləri:

- `animation-name` - Animasiyanın adını təyin edir.
- `animation-duration` - Animasiyanın davam etdiyi müddəti təyin edir.
- `animation-timing-function` - Animasiyanın davam etdiyi müddətin hər hansı bir funksiya ilə təyin edir.
- `animation-delay` - Animasiyanın başlama vaxtını təyin edir.
- `animation-iteration-count` - Animasiyanın təkrarlanma sayını təyin edir.
- `animation-direction` - Animasiyanın istiqamətini təyin edir.
- `animation-fill-mode` - Animasiyanın bitdikdəki vəziyyətini təyin edir.
- `animation-play-state` - Animasiyanın oynanma vəziyyətini təyin edir.

Nümunə:

```css
@keyframes example {
    0% {
        background-color: red;
    }
    50% {
        background-color: blue;
    }
    100% {
        background-color: green;
    }
}

div {
    animation-name: example;
    animation-duration: 4s;
    animation-timing-function: linear;
    animation-delay: 2s;
    animation-iteration-count: infinite;
    animation-direction: alternate;
    animation-fill-mode: forwards;
    animation-play-state: running;
}
```

Yuxarıdakı nümunədə, `@keyframes` rule ilə animasiyanın adı təyin edilir. `div` elementinə `animation` xüsusiyyəti ilə animasiya təyin edilir.