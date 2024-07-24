# HTML Dərs 3

## Formlar

Formlar, istifadəçilərin məlumat daxil etməsinə imkan verən HTML elementləridir. Formlar, məlumatları serverə göndərmək üçün istifadə olunur. Formlar, input, textarea, select, radio, checkbox, submit, reset, button və digər elementlərdən ibarətdir.

Form elementi, formun başlanğıcını və bitişini göstərir. Form elementinin action atributu, məlumatların göndərildiyi URL-ni göstərir. Method atributu isə məlumatların göndərilmə metodu təyin edir. Form elementinin içində input, textarea, select, radio, checkbox, submit, reset, button və digər elementlər yerləşdirilir.

Form elementi aşağıdakı kimi yazılır:

```html
<form action="URL" method="GET/POST">
	<!-- Form elementləri -->
</form>
```

### Caption elementi

Caption elementi, formun başlığını göstərir. Caption elementi, table elementinin içində yerləşdirilir. Caption elementi aşağıdakı kimi yazılır:

```html
<form action="URL" method="GET">
  <caption>Form başlığı</caption>
  <!-- Form elementləri -->
</form>
```

### Input elementi

Input elementi, istifadəçilərin məlumat daxil etməsinə imkan verən elementdir. Input elementinin type atributu, inputun növünü təyin edir. Input elementi aşağıdakı tiplərdə olur:

1. `<input type="text" name="" id=""/>` - mətn daxil etmək üçün istifadə olunur:

```html
<form action="URL" method="GET">
	<input type="text" name="username" id="username" />
	<input type="submit" value="Göndər" />
</form>
```

2. `<input type="password" name="" id=""/>` - şifrə daxil etmək üçün istifadə olunur:

```html
<form action="URL" method="GET">
	<input type="password" name="password" id="password" />
	<input type="submit" value="Göndər" />
</form>
```

3. `<input type="email" name="" id=""/>` - email daxil etmək üçün istifadə olunur:

```html
<form action="URL" method="GET">
	<input type="email" name="email" id="email" />
	<input type="submit" value="Göndər" />
</form>
```

4. `<input type="number" name="" id=""/>` - rəqəm daxil etmək üçün istifadə olunur:

```html
<form action="URL" method="GET">
	<input type="number" name="number" id="number" />
	<input type="submit" value="Göndər" />
</form>
```

5. `<input type="date" name="" id=""/>` - tarix daxil etmək üçün istifadə olunur:

```html
<form action="URL" method="GET">
	<input type="date" name="date" id="date" />
	<input type="submit" value="Göndər" />
</form>
```

6. `<input type="datetime-local" name="" id=""/>` - tarix və saat daxil etmək üçün istifadə olunur:

```html
<form action="URL" method="GET">
	<input type="datetime-local" name="datetime" id="datetime" />
	<input type="submit" value="Göndər" />
</form>
```

7. `<input type="radio" name="" id=""/>` - radio düyməsi yaratmaq üçün istifadə olunur:

```html
<form action="URL" method="GET">
	<input type="radio" name="radio" id="radio1" value="1" />1
	<input type="radio" name="radio" id="radio2" value="2" />2
	<input type="submit" value="Göndər" />
</form>

``` 

8. `<input type="checkbox" name="" id="" />` - checkbox yaratmaq üçün
istifadə olunur: 
```html
<form action="URL" method="GET">
	<input type="checkbox" name="checkbox" id="checkbox1" value="1" />1
	<input type="checkbox" name="checkbox" id="checkbox2" value="2" />2
	<input type="submit" value="Göndər" />
</form>

``` 

9. `<input type="submit" value="" />` - formu göndərmək üçün istifadə
olunur: 
```html
<form action="URL" method="GET">
	<input type="submit" value="Göndər" />
</form>

``` 

10. `<input type="reset" value="" />` - formdakı məlumatları silmək üçün
istifadə olunur: 
```html
<form action="URL" method="GET">
	<input type="reset" value="Sıfırla" />
</form>
```

11. `<input type="button" value=""/>` - düymə yaratmaq üçün istifadə olunur:

```html
<form action="URL" method="GET">
	<input type="button" value="Düymə" />
</form>

``` 

12. `<input type="file" name="" id="" />` - fayl yükləmək üçün istifadə
olunur: 

```html
<form action="URL" method="GET">
  <input type="file" name="file" id="file" />
  <input type="submit" value="Göndər" />
</form>
```

13. `<input type="hidden" name="" id="" />` - gizli məlumat göndərmək üçün
istifadə olunur: 

```html
<form action="URL" method="GET">
  <input type="hidden" name="hidden" id="hidden" value="Gizli məlumat" />
  <input type="submit" value="Göndər" />
</form>
```

14. `<input type="color" name="" id="" />` - rəng seçmək üçün istifadə
olunur: 

```html
<form action="URL" method="GET">
  <input type="color" name="color" id="color" />
  <input type="submit" value="Göndər" />
</form>
```

15. `<input type="range" name="" id="" />` - aralıq seçmək üçün istifadə
olunur: 

```html
<form action="URL" method="GET">
  <input type="range" name="range" id="range" />
  <input type="submit" value="Göndər" />
</form>
```

16. `<input type="tel" name="" id="" />` - telefon nömrəsi daxil etmək üçün
istifadə olunur: 

```html
<form action="URL" method="GET">
  <input type="tel" name="tel" id="tel" />
  <input type="submit" value="Göndər" />
</form>
```

17. `<input type="url" name="" id="" />` - URL daxil etmək üçün istifadə
olunur: 

```html
<form action="URL" method="GET">
  <input type="url" name="url" id="url" />
  <input type="submit" value="Göndər" />
</form>
```

18. `<input type="search" name="" id="" />` - axtarış etmək üçün istifadə
olunur: 

```html
<form action="URL" method="GET">
  <input type="search" name="search" id="search" />
  <input type="submit" value="Göndər" />
</form>
```

19. `<input type="time" name="" id="" />` - saat daxil etmək üçün istifadə
olunur: 

```html
<form action="URL" method="GET">
  <input type="time" name="time" id="time" />
  <input type="submit" value="Göndər" />
</form>
```

20. `<input type="week" name="" id="" />` - həftə seçmək üçün istifadə
olunur: 

```html
<form action="URL" method="GET">
  <input type="week" name="week" id="week" />
  <input type="submit" value="Göndər" />
</form>
```

21. `<input type="month" name="" id="" />` - ay seçmək üçün istifadə
olunur: 

```html
<form action="URL" method="GET">
  <input type="month" name="month" id="month" />
  <input type="submit" value="Göndər" />
</form>
```

22. `<input type="image" src="" alt="" />` - şəkil düyməsi yaratmaq üçün
istifadə olunur: 

```html
<form action="URL" method="GET">
  <input type="image" src="image.jpg" alt="Şəkil" />
</form>
```

### Textarea elementi

Textarea elementi, çoxlu sətirli mətn daxil etmək üçün istifadə olunur. Textarea elementinin rows və cols atributları, textarea elementinin hündürlüyünü və genişliyini təyin edir. Textarea elementi aşağıdakı kimi yazılır:

```html
<form action="URL" method="GET">
  <textarea name="message" id="message" rows="4" cols="50"></textarea>
  <input type="submit" value="Göndər" />
</form>
```

### Label elementi

Label elementi, input elementlərinin yanında mətn göstərmək üçün istifadə olunur. Label elementi, input elementləri ilə birgə istifadə olunur. Label elementi, for atributu ilə input elementinə bağlanır. Label elementi aşağıdakı kimi yazılır:

```html
<form action="URL" method="GET">
  <label for="username">İstifadəçi adı:</label>
  <input type="text" name="username" id="username" />
  <input type="submit" value="Göndər" />
</form>
```

### Select elementi

Select elementi, seçim elementləri yaratmaq üçün istifadə olunur. Select elementinin içində option elementləri yerləşdirilir. Option elementlərinin value atributu, seçim elementinin dəyərini təyin edir. Select elementi aşağıdakı kimi yazılır:

```html
<form action="URL" method="GET">
  <select name="city" id="city">
    <option value="baku">Bakı</option>
    <option value="ganja">Gəncə</option>
    <option value="sumgait">Sumqayıt</option>
  </select>
  <input type="submit" value="Göndər" />
</form>
```

### Fieldset elementi

Fieldset elementi, form elementlərini qruplaşdırmaq üçün istifadə olunur. Fieldset elementinin içində legend elementi yerləşdirilir. Legend elementi, fieldset elementinin başlığını göstərir. Fieldset elementi aşağıdakı kimi yazılır:

```html
<form action="URL" method="GET">
  <fieldset>
    <legend>Şəhər seçin</legend>
    <select name="city" id="city">
      <option value="baku">Bakı</option>
      <option value="ganja">Gəncə</option>
      <option value="sumgait">Sumqayıt</option>
    </select>
  </fieldset>
  <input type="submit" value="Göndər" />
</form>

```

### Datalist elementi

Datalist elementi, input elementləri üçün seçim elementləri yaratmaq üçün istifadə olunur. Datalist elementinin içində option elementləri yerləşdirilir. Datalist elementi aşağıdakı kimi yazılır:

```html
<form action="URL" method="GET">
  <input list="cities" name="city" id="city" />
  <datalist id="cities">
    <option value="Bakı"></option>
    <option value="Gəncə"></option>
    <option value="Sumqayıt"></option>
  </datalist>
  <input type="submit" value="Göndər" />
</form>

```

### Form elementinin atributları

1. `action` - Formun göndərildiyi URL-ni göstərir.
2. `method` - Formun göndərilmə metodu təyin edir. GET və POST olur.
3. `target` - Formun göndərildiyi URL-ni göstərir.
4. `autocomplete` - Form elementlərinin avtomatik doldurulmasını təyin edir.
5. `novalidate` - Form elementlərinin yoxlanılmasını deaktiv edir.
6. `enctype` - Formun göndərilmə metodu təyin edir.

### Input elementinin atributları

1. `type` - Input elementinin növünü təyin edir.
2. `name` - Input elementinin adını təyin edir.
3. `id` - Input elementinin id-sini təyin edir.
4. `value` - Input elementinin dəyərini təyin edir.
5. `placeholder` - Input elementinin placeholderini təyin edir.
6. `required` - Input elementinin doldurulması məcburidir.
7. `readonly` - Input elementinin dəyəri dəyişdirilməz.
8. `disabled` - Input elementi deaktiv edir.
9. `autofocus` - Input elementi avtomatik olaraq seçilir.
10. `multiple` - Input elementi çoxlu seçimə imkan verir.
11. `min` - Input elementinin minimum dəyərini təyin edir.
12. `max` - Input elementinin maksimum dəyərini təyin edir.
13. `step` - Input elementinin addımını təyin edir.
14. `pattern` - Input elementinin dəyərinin düzgün olub-olmadığını yoxlayır.
15. `form` - Input elementinin formunu təyin edir.
16. `formaction` - Input elementinin göndərildiyi URL-ni təyin edir.
17. `formenctype` - Input elementinin göndərilmə metodu təyin edir.
18. `formmethod` - Input elementinin göndərilmə metodu təyin edir.
19. `formnovalidate` - Input elementinin yoxlanılmasını deaktiv edir.
20. `formtarget` - Input elementinin göndərildiyi URL-ni təyin edir.

### Textarea elementinin atributları

1. `name` - Textarea elementinin adını təyin edir.
2. `id` - Textarea elementinin id-sini təyin edir.
3. `rows` - Textarea elementinin sətirlərinin sayını təyin edir.
4. `cols` - Textarea elementinin sütunlarının sayını təyin edir.
5. `placeholder` - Textarea elementinin placeholderini təyin edir.
6. `required` - Textarea elementinin doldurulması məcburidir.
7. `readonly` - Textarea elementinin dəyəri dəyişdirilməz.
8. `disabled` - Textarea elementi deaktiv edir.
9. `autofocus` - Textarea elementi avtomatik olaraq seçilir.
10. `form` - Textarea elementinin formunu təyin edir.

### Select elementinin atributları

1. `name` - Select elementinin adını təyin edir.
2. `id` - Select elementinin id-sini təyin edir.
3. `size` - Select elementinin seçim elementlərinin sayını təyin edir.
4. `multiple` - Select elementinin çoxlu seçimə imkan verir.
5. `required` - Select elementinin doldurulması məcburidir.
6. `disabled` - Select elementi deaktiv edir.
7. `autofocus` - Select elementi avtomatik olaraq seçilir.
8. `form` - Select elementinin formunu təyin edir.

### Option elementinin atributları

1. `value` - Option elementinin dəyərini təyin edir.
2. `selected` - Option elementi avtomatik olaraq seçilir.
3. `disabled` - Option elementi deaktiv edir.

### Button elementinin atributları

1. `name` - Button elementinin adını təyin edir.
2. `id` - Button elementinin id-sini təyin edir.
3. `value` - Button elementinin dəyərini təyin edir.
4. `type` - Button elementinin növünü təyin edir.
5. `form` - Button elementinin formunu təyin edir.
6. `formaction` - Button elementinin göndərildiyi URL-ni təyin edir.
7. `formenctype` - Button elementinin göndərilmə metodu təyin edir.
8. `formmethod` - Button elementinin göndərilmə metodu təyin edir.
9. `formnovalidate` - Button elementinin yoxlanılmasını deaktiv edir.
10. `formtarget` - Button elementinin göndərildiyi URL-ni təyin edir.


## CSS backgrounds

CSS-də background-color, background-image, background-repeat, background-attachment, background-position və digər background atributları istifadə olunur.

### background-color

Background-color atributu, elementin arxa fon rəngini təyin edir. Background-color atributu aşağıdakı kimi yazılır:

```css
body {
  background-color: lightblue;
}
```

### background-image

Background-image atributu, elementin arxa fon şəklini təyin edir. Background-image atributu aşağıdakı kimi yazılır:

```css
body {
  background-image: url('image.jpg');
}
```
və ya

```css
body {
  background-image: linear-gradient(to right, red, yellow);
}
```

və ya

```css
body {
  background-image: radial-gradient(circle, red, yellow);
}
```

və ya

```css
body {
  background: url('image.jpg')
}
```

### background-repeat

Background-repeat atributu, elementin arxa fon şəklinin təkrarlanma növünü təyin edir. 

1. repeat - Şəkil təkrarlanır.
2. repeat-x - Şəkil yalnız x oxu boyunca təkrarlanır.
3. repeat-y - Şəkil yalnız y oxu boyunca təkrarlanır.
4. no-repeat - Şəkil təkrarlanmır.

Background-repeat atributu aşağıdakı kimi yazılır:

```css
body {
  background-repeat: no-repeat;
}
```

### background-attachment

Background-attachment atributu, elementin arxa fon şəklinin səhifə ilə olan əlaqəsini təyin edir.

1. scroll - Şəkil səhifə ilə hərəkət edir.
2. fixed - Şəkil səhifə ilə hərəkət etmir.

Background-attachment atributu aşağıdakı kimi yazılır:

```css
body {
  background-attachment: fixed;
}
```

### background-position

Background-position atributu, elementin arxa fon şəklinin mövqeyini təyin edir. 

1. top - Şəkil yuxarıda olacaq.
2. bottom - Şəkil aşağıda olacaq.
3. left - Şəkil solda olacaq.
4. right - Şəkil sağda olacaq.
5. center - Şəkil mərkəzdə olacaq.
6. x% y% - Şəkilin mövqeyi yüz faizdə təyin edilir.
7. x-pos y-pos - Şəkilin mövqeyi pixel ilə təyin edilir.
8. top left - Şəkil yuxarı-solda olacaq.
9. top right - Şəkil yuxarı-sağda olacaq.
10. bottom left - Şəkil aşağı-solda olacaq.
11. bottom right - Şəkil aşağı-sağda olacaq.

Background-position atributu aşağıdakı kimi yazılır:

```css
body {
  background-position: center;
}
```

### background-size

Background-size atributu, elementin arxa fon şəklinin ölçüsünü təyin edir. 

1. auto - Şəkilin ölçüsü avtomatik olacaq.
2. length - Şəkilin ölçüsü pixel ilə təyin edilir.
3. percentage - Şəkilin ölçüsü yüz faizdə təyin edilir.
4. cover - Şəkilin ölçüsü elementin ölçüsünə uyğun olacaq.
5. contain - Şəkilin ölçüsü elementin ölçüsünə uyğun olacaq və şəkil tam olacaq.

Background-size atributu aşağıdakı kimi yazılır:

```css
body {
  background-size: cover;
}
```

### background-origin

Background-origin atributu, elementin arxa fon şəklinin başlanğıcını təyin edir. 

1. padding-box - Şəkil padding bölməsindən başlayacaq.
2. border-box - Şəkil border bölməsindən başlayacaq.
3. content-box - Şəkil məzmun bölməsindən başlayacaq.
4. initial - Şəkil default olaraq başlayacaq.

Background-origin atributu aşağıdakı kimi yazılır:

```css
body {
  background-origin: content-box;
}
```

### background-clip

Background-clip atributu, elementin arxa fon şəklinin məzmununu təyin edir. 

1. border-box - Şəkil border bölməsindən başlayacaq.
2. padding-box - Şəkil padding bölməsindən başlayacaq.
3. content-box - Şəkil məzmun bölməsindən başlayacaq.
4. initial - Şəkil default olaraq başlayacaq.

Background-clip atributu aşağıdakı kimi yazılır:

```css

body {
  background-clip: padding-box;
}
```

### background-shorthand

Background-shorthand atributu, elementin arxa fon atributlarını qısa formada təyin edir. Background-shorthand atributu aşağıdakı kimi yazılır:

```css

body {
  background: lightblue url('image.jpg') no-repeat fixed center/cover content-box padding-box;
}
```

## CSS borders

CSS-də border-width, border-style, border-color, border-radius və digər border atributları istifadə olunur.

### border-width

Border-width atributu, elementin sərhəd genişliyini təyin edir. Border-width atributu aşağıdakı kimi yazılır:

```css

div {
  border-width: 2px;
}
```

### border-style

Border-style atributu, elementin sərhəd növünü təyin edir. 

1. none - Sərhəd yoxdur.
2. hidden - Sərhəd gizlidir.
3. dotted - Sərhəd nöqtəli.
4. dashed - Sərhəd tireli.
5. solid - Sərhəd düz.
6. double - Sərhəd ikiqat.
7. groove - Sərhəd qıvrımlı.
8. ridge - Sərhəd yüksək.
9. inset - Sərhəd içəri.
10. outset - Sərhəd xarici.

Border-style atributu aşağıdakı kimi yazılır:

```css

div {
  border-style: solid;
}
```

### border-color

Border-color atributu, elementin sərhəd rəngini təyin edir. Border-color atributu aşağıdakı kimi yazılır:

```css

div {
  border-color: red;
}
```

### border-radius

Border-radius atributu, elementin sərhəd radiusunu təyin edir. Tam daire üçün border-radius: 50% yazılır. Border-radius atributu aşağıdakı kimi yazılır:

```css
div {
  border-radius: 10px;
}
```

### border-shorthand

Border-shorthand atributu, elementin sərhəd atributlarını qısa formada təyin edir. Border-shorthand atributu aşağıdakı kimi yazılır:

```css

div {
  border: 2px solid red;
}
```

## CSS margin

CSS-də margin-top, margin-right, margin-bottom, margin-left və digər margin atributları istifadə olunur.

### margin-top

Margin-top atributu, elementin üst marginini təyin edir. Margin-top atributu aşağıdakı kimi yazılır:

```css

div {
  margin-top: 10px;
}
```

### margin-right

Margin-right atributu, elementin sağ marginini təyin edir. Margin-right atributu aşağıdakı kimi yazılır:

```css

div {
  margin-right: 10px;
}
```

### margin-bottom

Margin-bottom atributu, elementin alt marginini təyin edir. Margin-bottom atributu aşağıdakı kimi yazılır:

```css

div {
  margin-bottom: 10px;
}
```

### margin-left

Margin-left atributu, elementin sol marginini təyin edir. Margin-left atributu aşağıdakı kimi yazılır:

```css

div {
  margin-left: 10px;
}
```

### margin-shorthand

Margin-shorthand atributu, elementin margin atributlarını qısa formada təyin edir. Margin-shorthand atributu aşağıdakı kimi yazılır:

```css

div {
  margin: 10px 20px 30px 40px;
}
```

## auto margin

Auto margin, elementin mərkəzə çəkilməsini təyin edir. Yalnız sağ və soldan ortalama üçün istifadə olunur. Yuxarı və aşağıdan ortalanmaya təsir etmir. Auto margin atributu aşağıdakı kimi yazılır:

```css
div {
  margin: 0 auto;
}
```

## CSS padding

CSS-də padding-top, padding-right, padding-bottom, padding-left və digər padding atributları istifadə olunur.

### padding-top

Padding-top atributu, elementin üst paddingini təyin edir. Padding-top atributu aşağıdakı kimi yazılır:

```css

div {
  padding-top: 10px;
}
```

### padding-right

Padding-right atributu, elementin sağ paddingini təyin edir. Padding-right atributu aşağıdakı kimi yazılır:

```css

div {
  padding-right: 10px;
}
```

### padding-bottom

Padding-bottom atributu, elementin alt paddingini təyin edir. Padding-bottom atributu aşağıdakı kimi yazılır:

```css

div {
  padding-bottom: 10px;
}
```

### padding-left

Padding-left atributu, elementin sol paddingini təyin edir. Padding-left atributu aşağıdakı kimi yazılır:

```css

div {
  padding-left: 10px;
}
```

### padding-shorthand

Padding-shorthand atributu, elementin padding atributlarını qısa formada təyin edir. Padding-shorthand atributu aşağıdakı kimi yazılır:

```css

div {
  padding: 10px 20px 30px 40px;
}
```

## CSS box model

CSS-də box model, elementin içində məzmun, padding, border və margin bölmələrini təyin edir. Box model, elementin ölçüsünü təyin edir. Yəni, elementin genişliyi və hündürlüyünü təyin edir.


```css

div {
  width: 100px;
  height: 100px;
  padding: 10px;
  border: 1px solid red;
  margin: 10px;
}
```

Yəni bu elementin yekun ölçüsü 122px olacaq. Çünki 100px məzmun, 10px padding, 1px border və 10px margin bölmələri var.

## CSS outline

CSS-də outline-width, outline-style, outline-color, outline-offset və digər outline atributları istifadə olunur.

### outline-width

Outline-width atributu, elementin sərhəd genişliyini təyin edir. Outline-width atributu aşağıdakı kimi yazılır:

```css
div {
  outline-width: 2px;
}
```

### outline-style

Outline-style atributu, elementin sərhəd növünü təyin edir. Outline-style atributu aşağıdakı kimi yazılır:

```css
div {
  outline-style: solid;
}
```

### outline-color

Outline-color atributu, elementin sərhəd rəngini təyin edir. Outline-color atributu aşağıdakı kimi yazılır:

```css
div {
  outline-color: red;
}
```

### outline-offset

Outline-offset atributu, elementin sərhəd aralığını təyin edir. Outline-offset atributu aşağıdakı kimi yazılır:

```css
div {
  outline-offset: 10px;
}
```

### outline-shorthand

Outline-shorthand atributu, elementin sərhəd atributlarını qısa formada təyin edir. Outline-shorthand atributu aşağıdakı kimi yazılır:

```css
div {
  outline: 2px solid red;
}
```

## box-sizing

Box-sizing atributu, elementin ölçüsünü təyin edir. Yəni elementin padding və border size-nı elementin ölçülərinin daxilində saxlayır.
Əgər box-sizing atributu content-box olarsa, elementin padding və border size-nı elementin ölçülərinin xaricində saxlayır və bu default dəyərdir. Box-sizing atributu aşağıdakı kimi yazılır:

```css
div {
  box-sizing: border-box;
}
```