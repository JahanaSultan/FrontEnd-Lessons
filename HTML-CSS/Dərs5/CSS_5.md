# CSS Dərs 5

## Box shadow

CSS box-shadow xüsusiyyəti elementin kölgəsini tənzimləmək üçün istifadə olunur. Elementin kölgəsini tənzimləmək üçün istifadə olunan box-shadow xüsusiyyeti bir sıra dəyərlərə malikdir. Bu dəyərlər:

- `horizontal` - Elementin kölgəsinin yatay istiqamətdə olan uzunluğunu təyin edir.
- `vertical` - Elementin kölgəsinin şaquli istiqamətdə olan uzunluğunu təyin edir.
- `blur` - Elementin kölgəsinin bulanıq olma dərəcəsini təyin edir.
- `spread` - Elementin kölgəsinin yayılma dərəcəsini təyin edir.
- `color` - Elementin kölgəsinin rəngini təyin edir.

Aşağıdakı şəkildə yazılır:

```css
div {
  box-shadow: 10px 10px 5px 0px rgba(0, 0, 0, 0.75);
}
```

Box shadow üçün generator: [https://www.cssmatic.com/box-shadow](https://www.cssmatic.com/box-shadow)
95 beautiful box shadow examples: [https://getcssscan.com/css-box-shadow-examples](https://getcssscan.com/css-box-shadow-examples)


## CSS display

CSS display xüsusiyyəti elementin görünüşünü tənzimləmək üçün istifadə olunur. Elementin görünüşünü dəyişdirmək üçün istifadə olunan display xüsusiyyəti bir sıra dəyərlərə malikdir. Bu dəyərlər:

- `block` - Elementi blok element kimi göstərir. Elementin sol və sağ küncündə boşluq yaranır.
- `inline` - Elementi inline element kimi göstərir. Elementin sol və sağ küncündə boşluq yaranmır.
- `inline-block` - Elementi inline-block element kimi göstərir. Elementin sol və sağ küncündə boşluq yaranmır.
- `none` - Elementi gizlədir.
- `flex` - Elementi flex element kimi göstərir.
- `grid` - Elementi grid element kimi göstərir.

`inline` və `inline-block` dəyərləri arasındakı fərqi aşağıdakı şəkildə izah edə bilərik:

- `inline` elementlərə `width` və `height` təyin edilə bilmir.
- `inline-block` elementlərə `width` və `height` təyin edilə bilir.

Yəni `inline-block` elementlər `inline` elementlər kimi yan-yana sıralana `block` elementlər kimi ölçüləndirilə bilir.

Aşağıdakı şəkildə yazılır:

```css
div {
  display: block;
}
```

## Flexbox

Flexbox CSS modulu, elementlərin sıralanmasını və yerləşməsini tənzimləmək üçün istifadə olunan bir CSS moduludur. Flexbox modulu, elementləri sıralamaq və yerləşdirmək üçün ən rahat yoldur. Flexbox modulu, elementləri sıralamaq və yerləşdirmək üçün istifadə olunan bir çox xüsusiyyətlərə malikdir. Bu xüsusiyyətlər:

- `flex-direction` - Elementlərin sıralanma istiqamətini təyin edir.
- `flex-wrap` - Elementlərin sıralanma qaydasını təyin edir.
- `justify-content` - Elementlərin sıralanma istiqamətindən asılı olaraq elementlərin sağ və sol küncündə boşluq yaradır.
- `align-items` - Elementlərin sıralanma istiqamətindən asılı olaraq elementlərin üst və alt küncündə boşluq yaradır.
- `align-content` - Elementlərin sıralanma istiqamətindən asılı olaraq elementlərin üst və alt küncündə boşluq yaradır.
- `flex-flow` - `flex-direction` və `flex-wrap` xüsusiyyətlərini eyni anda təyin etmək üçün istifadə olunur.
- `align-self` - Elementin özünə məxsus `align-items` xüsusiyyətini təyin etmək üçün istifadə olunur.
- `order` - Elementlərin sıralanma qaydasını təyin etmək üçün istifadə olunur.
- `flex-grow` - Elementin ölçüsünü artırmaq üçün istifadə olunur.
- `flex-shrink` - Elementin ölçüsünü azaltmaq üçün istifadə olunur.
- `flex-basis` - Elementin ölçüsünü təyin etmək üçün istifadə olunur.
- `flex` - `flex-grow`, `flex-shrink` və `flex-basis` xüsusiyyətlərini eyni anda təyin etmək üçün istifadə olunur.
- `gap` - Elementlər arasında boşluq yaradır.

Aşağıdakı şəkildə yazılır:

```css
.container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
```

### Flexbox özəllikləri

1. `flex-direction` xüsusiyyəti:

- `row` -  Elementlər soldan sağa doğru sıralanır.
- `row-reverse` -  Elementlər sağdan sola doğru sıralanır.
- `column` -  Elementlər yuxarıdan aşağıya doğru sıralanır.
- `column-reverse` -  Elementlər aşağıdan yuxarıya doğru sıralanır.

2. `flex-wrap` xüsusiyyəti:

- `nowrap` -  Elementlər bir sıradan başqa sıraya keçməz.
- `wrap` -  Elementlər bir sıradan başqa sıraya keçə bilər.
- `wrap-reverse` -  Elementlər bir sıradan başqa sıraya keçə bilər, amma sıralar tərsinə sıralanır.

3. `justify-content` xüsusiyyəti:

- `flex-start` -  Elementlər sıranın sol küncündə yerləşir.
- `flex-end` -  Elementlər sıranın sağ küncündə yerləşir.
- `center` -  Elementlər sıranın ortasında yerləşir.
- `space-between` -  Elementlər arasında boşluq yaranır.
- `space-around` -  Elementlər arasında və sıranın sağ və sol küncündə boşluq yaranır.

4. `align-items` xüsusiyyəti:

- `flex-start` -  Elementlər sıranın üst küncündə yerləşir.
- `flex-end` -  Elementlər sıranın alt küncündə yerləşir.
- `center` -  Elementlər sıranın ortasında yerləşir.
- `baseline` -  Elementlər sıranın bazasında yerləşir.
- `stretch` -  Elementlər sıranın hər iki küncündə yerləşir.

5. `align-content` xüsusiyyəti:

- `flex-start` -  Elementlər sıranın üst küncündə yerləşir.
- `flex-end` -  Elementlər sıranın alt küncündə yerləşir.
- `center` -  Elementlər sıranın ortasında yerləşir.
- `space-between` -  Elementlər arasında boşluq yaranır.
- `space-around` -  Elementlər arasında və sıranın üst və alt küncündə boşluq yaranır.
- `stretch` -  Elementlər sıranın hər iki küncündə yerləşir.

6. `align-self` xüsusiyyəti:

- `auto` -  Elementin özünə məxsus `align-items` xüsusiyyətini təyin edir.
- `flex-start` -  Element sıranın üst küncündə yerləşir.
- `flex-end` -  Element sıranın alt küncündə yerləşir.
- `center` -  Element sıranın ortasında yerləşir.
- `baseline` -  Element sıranın bazasında yerləşir.
- `stretch` -  Element sıranın hər iki küncündə yerləşir.

7. `order` xüsusiyyəti:

- `0` -  Elementin sıralanma qaydasını dəyişdirmir.
- `1` -  Elementi bir sıra aşağıya salır.
- `2` -  Elementi iki sıra aşağıya salır.
- `-1` -  Elementi bir sıra yuxarıya qaldırır.
- `-2` -  Elementi iki sıra yuxarıya qaldırır.

8. `flex-grow` xüsusiyyəti:

- `0` -  Elementin ölçüsünü artırmır.
- `1` -  Elementin ölçüsünü artırır.

9. `flex-shrink` xüsusiyyəti:

- `0` -  Elementin ölçüsünü azaltmır.
- `1` -  Elementin ölçüsünü azaldır.

10. `flex-basis` xüsusiyyəti:

- `auto` -  Elementin ölçüsünü avtomatik olaraq təyin edir.
- `100px` -  Elementin ölçüsünü 100 piksel olaraq təyin edir.

11. `flex` xüsusiyyəti:

- `1 1 100px` -  `flex-grow`, `flex-shrink` və `flex-basis` xüsusiyyətlərini eyni anda təyin edir. Bu o deməkdir ki, elementin ölçüsü 100 piksel olacaq və ölçüsü 100 pikseldən az olmamaq şərti ilə arta biləcək və azala biləcək.

## max-width və min-width

`max-width` və `min-width` xüsusiyyətləri elementin maksimum və minimum ölçüsünü təyin etmək üçün istifadə olunur. `max-width` xüsusiyyəti elementin maksimum ölçüsünü təyin edir. `min-width` xüsusiyyəti elementin minimum ölçüsünü təyin edir.

Aşağıdakı şəkildə yazılır:

```css
div {
  max-width: 100px;
  min-width: 50px;
}
```

## max-height və min-height

`max-height` və `min-height` xüsusiyyətləri elementin maksimum və minimum hündürlüyünü təyin etmək üçün istifadə olunur. `max-height` xüsusiyyəti elementin maksimum hündürlüyünü təyin edir. `min-height` xüsusiyyəti elementin minimum hündürlüyünü təyin edir.

Aşağıdakı şəkildə yazılır:

```css
div {
  max-height: 100px;
  min-height: 50px;
}
```

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

1. [https://eco-nature.cmsmasters.net/](https://eco-nature.cmsmasters.net/) saytının Header hissəsini yığın.