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


# Tapşırıq

1. [https://eco-nature.cmsmasters.net/](https://eco-nature.cmsmasters.net/) saytının Header hissəsini yığın.