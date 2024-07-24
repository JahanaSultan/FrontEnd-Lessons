# CSS Dərs 4

## CSS text

CSS text xüsusiyyətləri mətnin görünüşünü tənzimləmək üçün istifadə olunur.

### text-align

Mətnin hərəkətini tənzimləmək üçün istifadə olunur.

1. `left` - Mətni sola çəkir.
2. `right` - Mətni sağa çəkir.
3. `center` - Mətni mərkəzə çəkir.
4. `justify` - Mətni sətirin hər iki tərəfinə çəkir.

Aşağıdakı şəkildə yazılır:

```css
p {
  text-align: center;
}
```

### text-decoration

Mətnin üzərindəki süslemələri tənzimləmək üçün istifadə olunur.

1. `none` - Hər hansı bir süslemə olmur.
2. `underline` - Mətnin altını xəttlə çəkir.
3. `overline` - Mətnin üstünü xəttlə çəkir.
4. `line-through` - Mətnin ortasından xəttlə çəkir.
5. `blink` - Mətni süzgəc ilə işıqlandırır.

Aşağıdakı şəkildə yazılır:

```css
p {
  text-decoration: underline;
}
```

### text-transform

Mətnin hərflərinin böyüklüyünü tənzimləmək üçün istifadə olunur.

1. `none` - Hərflər normal görünür.
2. `uppercase` - Hərflər böyük görünür.
3. `lowercase` - Hərflər kiçik görünür.
4. `capitalize` - Hər bir sözün ilk hərfi böyük görünür.

Aşağıdakı şəkildə yazılır:

```css
p {
  text-transform: uppercase;
}
```

### text-indent

Mətnin solundan boşluğu tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
p {
  text-indent: 50px;
}
```

### line-height

Mətnin sətirlərinin arasındakı boşluğu tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
p {
  line-height: 1.5;
}
```

### letter-spacing

Mətnin hərflərinin arasındakı boşluğu tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
p {
  letter-spacing: 2px;
}
```

### word-spacing

Mətnin sözlərinin arasındakı boşluğu tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
p {
  word-spacing: 5px;
}
```

### text-shadow

Mətnin gölgəsini tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
p {
  text-shadow: 2px 2px 5px red;
}
```

### white-space

Mətnin boşluqlarını tənzimləmək üçün istifadə olunur.

1. `normal` - Mətnin boşluqlarını normal göstərir.
2. `nowrap` - Mətnin boşluqlarını olmadan göstərir.
3. `pre` - Mətnin boşluqlarını saxlayaraq göstərir.
4. `pre-line` - Mətnin boşluqlarını saxlayaraq göstərir və sətirləri saxlayaraq göstərir.
5. `pre-wrap` - Mətnin boşluqlarını saxlayaraq göstərir və sətirləri saxlayaraq göstərir.

Aşağıdakı şəkildə yazılır:

```css
p {
  white-space: nowrap;
}
```

### word-wrap

Mətnin sözlərinin sətirin sonuna çatdıqda qırılmasını tənzimləmək üçün istifadə olunur.

1. `normal` - Söz sətirin sonuna çatdıqda qırılmır.
2. `break-word` - Söz sətirin sonuna çatdıqda qırılır.
3. `initial` - Standart dəyər.

Aşağıdakı şəkildə yazılır:

```css
p {
  word-wrap: break-word;
}
```

### word-break

Mətnin sözlərinin sətirin sonuna çatdıqda qırılmasını tənzimləmək üçün istifadə olunur.

1. `normal` - Söz sətirin sonuna çatdıqda qırılmır.
2. `break-all` - Söz sətirin sonuna çatdıqda qırılır.
3. `keep-all` - Söz sətirin sonuna çatdıqda qırılmır.
4. `initial` - Standart dəyər.

Aşağıdakı şəkildə yazılır:

```css
p {
  word-break: break-all;
}
```

### direction

Mətnin istiqamətini tənzimləmək üçün istifadə olunur.

1. `ltr` - Mətni sola doğru yazır.
2. `rtl` - Mətni sağa doğru yazır.

Aşağıdakı şəkildə yazılır:

```css
p {
  direction: rtl;
}
```

### unicode-bidi

Mətnin yazılış istiqamətini tənzimləmək üçün istifadə olunur və `direction` xüsusiyyəti ilə birlikdə istifadə olunur.

1. `normal` - Standart dəyər.
2. `embed` - Mətnin yazılış istiqamətini tənzimləyir.
3. `bidi-override` - Mətnin yazılış istiqamətini tənzimləyir.
4. `initial` - Standart dəyər.

Aşağıdakı şəkildə yazılır:

```css
p {
  direction: rtl;
  unicode-bidi: bidi-override;
}
```

### text-overflow

Mətnin sətirin sonuna çatdıqda nə olacağını tənzimləmək üçün istifadə olunur.

1. `clip` - Mətni kəsir.
2. `ellipsis` - Mətnin sonuna üç nöqtə qoyur.
3. `string` - Mətnin sonuna istənilən mətni qoyur.

Aşağıdakı şəkildə yazılır:

```css
p {
  text-overflow: ellipsis;
}
```

### overflow-wrap

Mətnin sətirin sonuna çatdıqda nə olacağını tənzimləmək üçün istifadə olunur.

1. `normal` - Söz sətirin sonuna çatdıqda qırılmır.
2. `break-word` - Söz sətirin sonuna çatdıqda qırılır.
3. `anywhere` - Söz sətirin sonuna çatdıqda qırılmır.
4. `initial` - Standart dəyər.

Aşağıdakı şəkildə yazılır:

```css
p {
  overflow-wrap: break-word;
}
```

### text-align-last

Mətnin son sətirini tənzimləmək üçün istifadə olunur.

1. `auto` - Standart dəyər.
2. `left` - Mətni sola çəkir.
3. `right` - Mətni sağa çəkir.

Aşağıdakı şəkildə yazılır:

```css
p {
  text-align-last: right;
}
```

## Font

### font-family

Mətnin fontunu tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
p {
  font-family: Arial, sans-serif;
}
```

### font-size

Mətnin ölçüsünü tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
p {
  font-size: 16px;
}
```

### font-style

Mətnin stili tənzimləmək üçün istifadə olunur.

1. `normal` - Standart dəyər.
2. `italic` - Mətni italik görünür.
3. `oblique` - Mətni oblik görünür.

Aşağıdakı şəkildə yazılır:

```css
p {
  font-style: italic;
}
```

### font-weight

Mətnin qalın olub olmamasını tənzimləmək üçün istifadə olunur.

1. `normal` - Standart dəyər.
2. `bold` - Mətn qalındır.
3. `bolder` - Mətn daha qalındır.
4. `lighter` - Mətn daha kiçikdir.
5. `100` - 900 - Mətnin qalınlığını tənzimləyir.

Aşağıdakı şəkildə yazılır:

```css
p {
  font-weight: bold;
}
```

### font-variant

Mətnin variantını tənzimləmək üçün istifadə olunur.

1. `normal` - Standart dəyər.
2. `small-caps` - Mətnin hərfləri kiçik böyük görünür.

Aşağıdakı şəkildə yazılır:

```css
p {
  font-variant: small-caps;
}
```

### font-stretch

Mətnin genişliyini tənzimləmək üçün istifadə olunur və `font-family` xüsusiyyəti ilə birlikdə istifadə olunur.

1. `normal` - Standart dəyər.
2. `ultra-condensed` - Mətnin genişliyi çox kiçikdir.
3. `extra-condensed` - Mətnin genişliyi kiçikdir.
4. `condensed` - Mətnin genişliyi kiçikdir.
5. `semi-condensed` - Mətnin genişliyi kiçikdir.
6. `semi-expanded` - Mətnin genişliyi böyükdür.
7. `expanded` - Mətnin genişliyi böyükdür.
8. `extra-expanded` - Mətnin genişliyi böyükdür.
9. `ultra-expanded` - Mətnin genişliyi çox böyükdür.

Aşağıdakı şəkildə yazılır:

```css
p {
  font-family: Arial, sans-serif;
  font-stretch: ultra-expanded;
}
```

### Google Fonts

Google Fonts saytından istənilən fontu seçib istifadə edə bilərsiniz. [Google Fonts](https://fonts.google.com/)

### @font-face

Öz fontunuzu yaratmaq üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
@font-face {
  font-family: "MyFont";
  src: url("myfont.woff");
}
```

## Icons

İkonlar saytın görsənəkliyini artırmaq üçün istifadə olunur.

### Font Awesome

Font Awesome saytından istənilən ikonu seçib istifadə edə bilərsiniz. [Font Awesome](https://fontawesome.com/)

### Ionicons

Ionicons saytından istənilən ikonu seçib istifadə edə bilərsiniz. [Ionicons](https://ionicons.com/)

### Remix Icon

Remix Icon saytından istənilən ikonu seçib istifadə edə bilərsiniz. [Remix Icon](https://remixicon.com/)

### Feather Icons

Feather Icons saytından istənilən ikonu seçib istifadə edə bilərsiniz. [Feather Icons](https://feathericons.com/)

### Heroicons

Heroicons saytından istənilən ikonu seçib istifadə edə bilərsiniz. [Heroicons](https://heroicons.com/)

### Tabler Icons

Tabler Icons saytından istənilən ikonu seçib istifadə edə bilərsiniz. [Tabler Icons](https://tablericons.com/)

## Links

Linkləri tənzimləmək üçün bir sıra xüsusiyyətlər mövcuddur.

### a:link

Linkin standart görünüşünü tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
a:link {
  color: blue;
}
```

### a:visited

Linkə klikləndikdən sonra görünüşünü tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
a:visited {
  color: purple;
}
```

### a:hover

Linkə mouse ilə getdikdə görünüşünü tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
a:hover {
  color: red;
}
```

### a:active

Linkə klikləndikdə görünüşünü tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
a:active {
  color: green;
}
```

## Lists

### list-style-type

Listin növünü tənzimləmək üçün istifadə olunur.

1. `none` - Listin növü olmur.
2. `disc` - Listin növü diskdir.
3. `circle` - Listin növü çevrədir.
4. `square` - Listin növü kvadratdır.
5. `decimal` - Listin növü rəqəmdir.
6. `decimal-leading-zero` - Listin növü rəqəmdir və 0 ilə başlayır.
7. `lower-roman` - Listin növü kiçik roman rəqəmləridir.
8. `upper-roman` - Listin növü böyük roman rəqəmləridir.
9. `lower-alpha` - Listin növü kiçik hərflərdən ibarətdir.
10. `upper-alpha` - Listin növü böyük hərflərdən ibarətdir.

Aşağıdakı şəkildə yazılır:

```css
ul {
  list-style-type: square;
}
```

### list-style-position

Listin növünün mövqeyini tənzimləmək üçün istifadə olunur.

1. `inside` - Listin növü listin içindədir.
2. `outside` - Listin növü listin xaricindədir.

Aşağıdakı şəkildə yazılır:

```css
ul {
  list-style-position: inside;
}
```

### list-style-image

Listin növünü şəkil ilə tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
ul {
  list-style-image: url('image.png');
}
```

## Tables

### table

Cədvəlin ümumi xüsusiyyətlərini tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
table {
  width: 100%;
  border-collapse: collapse;
}
```

`border-collapse` xüsusiyyəti iki dəyər qəbul edir:

1. `separate` - Cədvəl sətirləri və sütunları ayrı-ayrıdır.
2. `collapse` - Cədvəl sətirləri və sütunları bir-birinə yapışıqdır.

### th

Cədvəlin başlıqlarını tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
th {
  background-color: #f2f2f2;
  color: black;
}
```

### td

Cədvəlin məlumatlarını tənzimləmək üçün istifadə olunur.

Aşağıdakı şəkildə yazılır:

```css
td {
  border: 1px solid #dddddd;
  text-align: left;
  padding: 8px;
}
```