# CSS Dərs 6


## CSS position

CSS position xüsusiyyəti elementin mövqeyini tənzimləmək üçün istifadə olunur. Elementin mövqeyini tənzimləmək üçün istifadə olunan position xüsusiyyəti bir sıra dəyərlərə malikdir. Bu dəyərlər:

- `static` - Elementin mövqeyi normal mövqeyindədir.
- `relative` - Elementin mövqeyi öz mövqeyindədir.
- `absolute` - Elementin mövqeyi elementin üst elementinə nisbətən təyin edilir.
- `fixed` - Elementin mövqeyi səhifəyə nisbətən təyin edilir.
- `sticky` - Elementin mövqeyi səhifəyə nisbətən təyin edilir, amma səhifə scroll olunduqda element səhifənin üstündə qalır.

Aşağıdakı şəkildə yazılır:

```css
div {
  position: relative;
}

div {
  position: absolute;
  top: 0;
  left: 0;
}
```

Bu kodda, `position: relative;` xüsusiyyəti elementin mövqeyini öz mövqeyində təyin edir. `position: absolute;` xüsusiyyəti elementin mövqeyini elementin üst elementinə nisbətən təyin edir. `top: 0;` və `left: 0;` xüsusiyyətləri elementin mövqeyini səhifənin sol üst küncündə təyin edir.

## CSS z-index

CSS z-index xüsusiyyəti elementlərin üst-üstə gəlməsinin qaydasını tənzimləmək üçün istifadə olunur. Elementlərin üst-üstə gəlməsinin qaydasını tənzimləmək üçün istifadə olunan z-index xüsusiyyəti bir tam ədəd dəyərə malikdir. Ədəd dəyəri çoxlu elementlərin üst-üstə gəlməsinin qaydasını təyin edir. Ədəd dəyəri kiçik olan elementlər ən üstə, ədəd dəyəri böyük olan elementlər ən alta düşür.

Aşağıdakı şəkildə yazılır:

```css
div {
  z-index: 1;
}
```

Bu kodda, `z-index: 1;` xüsusiyyəti elementin z-index dəyərini 1 ədədində təyin edir.

## CSS overflow

CSS overflow xüsusiyyəti elementin içərisindəki məzmunun görünüşünü tənzimləmək üçün istifadə olunur. Elementin içərisindəki məzmunun görünüşünü tənzimləmək üçün istifadə olunan overflow xüsusiyyəti bir sıra dəyərlərə malikdir. Bu dəyərlər:

- `visible` - Elementin içərisindəki məzmun görünürdür.
- `hidden` - Elementin içərisindəki məzmun gizlənir.
- `scroll` - Elementin içərisindəki məzmun scroll olunur.
- `auto` - Elementin içərisindəki məzmun avtomatik olaraq scroll olunur.

Aşağıdakı şəkildə yazılır:

```css
div {
  overflow: hidden;
}
```

Bu kodda, `overflow: hidden;` xüsusiyyəti elementin içərisindəki məzmunun gizlənəcəyini təyin edir.

### CSS overflow-x və overflow-y

- `overflow-x` - Elementin içərisindəki məzmunun üfüqi scroll olunmasını tənzimləmək üçün istifadə olunur.
- `overflow-y` - Elementin içərisindəki məzmunun şaquli scroll olunmasını tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
div {
  overflow-x: hidden;
  overflow-y: scroll;
}
```

## CSS float

CSS float xüsusiyyəti elementin sağ və sol küncündən səhifənin sağ və sol küncünə doğru sürüşməsini tənzimləmək üçün istifadə olunur. Elementin sağ və sol küncündən səhifənin sağ və sol küncünə doğru sürüşməsini tənzimləmək üçün istifadə olunan float xüsusiyyeti bir sıra dəyərlərə malikdir. Bu dəyərlər:

- `left` - Element səhifənin sol küncündən sağ küncünə doğru yüzer.
- `right` - Element səhifənin sağ küncündən sol küncünə doğru yüzer.
- `none` - Element yüzmür.

Aşağıdakı şəkildə yazılır:

```css
div {
  float: left;
}
```

## CSS clear

CSS clear xüsusiyyəti elementin sürüşdüyü elementlərin yanına düşməməsini tənzimləmək üçün istifadə olunur. Elementin sürüşdüyü elementlərin yanına düşməməsini tənzimləmək üçün istifadə olunan clear xüsusiyyeti bir sıra dəyərlərə malikdir. Bu dəyərlər:

- `left` - Elementin sol küncündən sürüşdüyü elementlərin yanına düşməməsini təyin edir.
- `right` - Elementin sağ küncündən sürüşdüyü elementlərin yanına düşməməsini təyin edir.
- `both` - Elementin hər iki küncündən sürüşdüyü elementlərin yanına düşməməsini təyin edir.
- `none` - Elementin sürüşdüyü elementlərin yanına düşməsini təyin edir.

Aşağıdakı şəkildə yazılır:

```css
div {
  clear: left;
}
```

## CSS opacity

CSS opacity xüsusiyyəti elementin şəffaflığını tənzimləmək üçün istifadə olunur. Elementin şəffaflığını tənzimləmək üçün istifadə olunan opacity xüsusiyyeti bir ədəd dəyərə malikdir. Ədəd dəyəri 0 ilə 1 arasında olur. 0 dəyəri elementin şəffaflığını təyin edir. 1 dəyəri elementin şəffaflığını təyin etmir.

Aşağıdakı şəkildə yazılır:

```css
div {
  opacity: 0.5;
}
```

Bu kodda, `opacity: 0.5;` xüsusiyyəti elementin şəffaflığını 0.5 ədədində təyin edir.

## CSS transition

CSS transition xüsusiyyəti elementin dəyişmə effektlərini tənzimləmək üçün istifadə olunur. Elementin dəyişmə effektlərini tənzimləmək üçün istifadə olunan transition xüsusiyyeti bir sıra dəyərlərə malikdir. Bu dəyərlər:

- `property` - Elementin dəyişmə effektlərini təyin edir.
- `duration` - Elementin dəyişmə effektlərinin davam etdiyi müddəti təyin edir.
- `timing-function` - Elementin dəyişmə effektlərinin davranışını təyin edir.
- `delay` - Elementin dəyişmə effektlərinin başlama vaxtını təyin edir.

Aşağıdakı şəkildə yazılır:

```css
div {
  transition: width 2s ease 1s;
}
```

Bu kodda, `transition: width 2s ease 1s;` xüsusiyyəti elementin genişliyinin 2 saniyə davam etdiyi, davranışının ease olduğu və 1 saniyə sonra başladığı təyin edilir.

## CSS combinators

CSS combinators CSS seçicilərini bir-birilərinə birləşdirmək üçün istifadə olunur. CSS seçicilərini bir-birilərinə birləşdirmək üçün istifadə olunan combinators bir sıra dəyərlərə malikdir. Bu dəyərlər:

- ` ` - Boşluq seçicisi. Bu seçici elementin içində olan elementləri seçir.
- `>` - Child seçicisi. Bu seçici elementin birinci child elementini seçir.
- `+` - Adjacent sibling seçicisi. Bu seçici elementin birinci qardaşı elementini seçir.
- `~` - General sibling seçicisi. Bu seçici elementin qardaşı elementlərini seçir.

Aşağıdakı şəkildə yazılır:

```css
div p {
  color: red;
}

div > p {
  color: blue;
}

div + p {
  color: green;
}

div ~ p {
  color: yellow;
}
```

Bu kodda, `div p` seçicisi div elementinin içində olan p elementlərini seçir. `div > p` seçicisi div elementinin birinci child p elementini seçir. `div + p` seçicisi div elementinin birinci qardaşı p elementini seçir. `div ~ p` seçicisi div elementinin qardaşı p elementlərini seçir.

## CSS attribute selectors

CSS attribute selectors CSS seçicilərini elementin atributlarına görə seçmək üçün istifadə olunur. Elementin atributlarına görə seçmək üçün istifadə olunan attribute selectors bir sıra dəyərlərə malikdir. Bu dəyərlər:

- `[attribute]` - Elementin atributlarından biri olan attribute atributuna sahib elementləri seçir.
- `[attribute=value]` - Elementin atributlarından biri olan attribute atributu dəyəri value olan elementləri seçir.
- `[attribute~=value]` - Elementin atributlarından biri olan attribute atributu dəyəri value olan elementləri seçir. Dəyər value dəyəri ilə eyni olmalıdır.
- `[attribute|=value]` - Elementin atributlarından biri olan attribute atributu dəyəri value olan elementləri seçir. Dəyər value dəyəri ilə eyni olmalıdır və ya value-dən sonra `-` işarəsi olmalıdır.
- `[attribute^=value]` - Elementin atributlarından biri olan attribute atributu dəyəri value ilə başlayan elementləri seçir.
- `[attribute$=value]` - Elementin atributlarından biri olan attribute atributu dəyəri value ilə bitən elementləri seçir.
- `[attribute*=value]` - Elementin atributlarından biri olan attribute atributu dəyəri value olan elementləri seçir. Dəyər value dəyəri ilə eyni olmalıdır.

Aşağıdakı şəkildə yazılır:

```css
div[class] {
  color: red;
}

div[class="container"] {
  color: blue;
}

div[class~="container"] {
  color: green;
}

div[class|="container"] {
  color: yellow;
}

div[class^="container"] {
  color: orange;
}

div[class$="container"] {
  color: purple;
}

div[class*="container"] {
  color: pink;
}
```

Bu kodda, `div[class]` seçicisi div elementinin class atributuna sahib elementləri seçir. `div[class="container"]` seçicisi div elementinin class atributu container olan elementləri seçir. `div[class~="container"]` seçicisi div elementinin class atributu container olan elementləri seçir. `div[class|="container"]` seçicisi div elementinin class atributu container olan elementləri seçir. `div[class^="container"]` seçicisi div elementinin class atributu container ilə başlayan elementləri seçir. `div[class$="container"]` seçicisi div elementinin class atributu container ilə bitən elementləri seçir. `div[class*="container
"]` seçicisi div elementinin class atributu container olan elementləri seçir.

## CSS filters

CSS filters CSS elementlərinin görünüşünü tənzimləmək üçün istifadə olunur. Elementlərin görünüşünü tənzimləmək üçün istifadə olunan filters bir sıra dəyərlərə malikdir. Bu dəyərlər:

- `blur()` - Elementin bulanıq olma dərəcəsini təyin edir.
- `brightness()` - Elementin işıq dərəcəsini təyin edir.
- `contrast()` - Elementin kontrast dərəcəsini təyin edir.
- `drop-shadow()` - Elementin kölgəsini təyin edir.
- `grayscale()` - Elementin siyahı rəngində olma dərəcəsini təyin edir.
- `hue-rotate()` - Elementin rəngini döndürür.
- `invert()` - Elementin rənglərini dəyişdirir.
- `opacity()` - Elementin şəffaflığını təyin edir.
- `saturate()` - Elementin doyma dərəcəsini təyin edir.
- `sepia()` - Elementin sepia rəngində olma dərəcəsini təyin edir.

Aşağıdakı şəkildə yazılır:

```css
div {
  filter: blur(5px);
}
```

Bu kodda, `filter: blur(5px);` xüsusiyyəti elementin bulanıq olma dərəcəsini 5 piksel olaraq təyin edir.


## CSS object-fit

CSS object-fit xüsusiyyəti elementin ölçüsünü tənzimləmək üçün istifadə olunur. Elementin ölçüsünü tənzimləmək üçün istifadə olunan object-fit xüsusiyyeti bir sıra dəyərlərə malikdir. Bu dəyərlər:

- `fill` - Elementin ölçüsünü dəyişdirmədən elementi ölçüsünə uyğunlaşdırır.
- `contain` - Elementin ölçüsünü dəyişdirmədən elementi ölçüsünə uyğunlaşdırır və elementin hər iki küncündən boşluq yaranır.
- `cover` - Elementin ölçüsünü dəyişdirmədən elementi ölçüsünə uyğunlaşdırır və elementin hər iki küncündən boşluq yaranmır.
- `none` - Elementin ölçüsünü dəyişdirmədən elementi ölçüsünə uyğunlaşdırır və elementin hər iki küncündən boşluq yaranmır.
- `scale-down` - Elementin ölçüsünü dəyişdirmədən elementi ölçüsünə uyğunlaşdırır və elementin hər iki küncündən boşluq yaranır.

Aşağıdakı şəkildə yazılır:

```css
img {
  object-fit: cover;
}
```

Bu kodda, `object-fit: cover;` xüsusiyyəti img elementinin ölçüsünü dəyişdirmədən elementi ölçüsünə uyğunlaşdırır və elementin hər iki küncündən boşluq yaranmır.

# Tapşırıq

1. [https://preview.themeforest.net/item/leadengine-multipurpose-wordpress-theme-with-page-builder/full_screen_preview/21514338?clickid=wxG0TM0lYxyPR-T2ChRT4yB4UkCz0z2P4SaFWc0&iradid=275988&iradtype=ONLINE_TRACKING_LINK&irgwc=1&irmptype=mediapartner&irpid=369282&mp_value1=&utm_campaign=af_impact_radius_369282&utm_medium=affiliate&utm_source=impact_radius](https://preview.themeforest.net/item/leadengine-multipurpose-wordpress-theme-with-page-builder/full_screen_preview/21514338?clickid=wxG0TM0lYxyPR-T2ChRT4yB4UkCz0z2P4SaFWc0&iradid=275988&iradtype=ONLINE_TRACKING_LINK&irgwc=1&irmptype=mediapartner&irpid=369282&mp_value1=&utm_campaign=af_impact_radius_369282&utm_medium=affiliate&utm_source=impact_radius) saytının "Qualified doctors" hissəsinə qədər yığın.