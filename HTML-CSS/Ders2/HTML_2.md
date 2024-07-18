# HTML Dərs 2

## HTML video və audio

HTML video və audio elementləri, səhifədə video və səs fayllarını göstərmək üçün istifadə olunur. HTML video və audio elementləri, `<video>` və `<audio>` etiketləri ilə təyin olunur və `src` atributu ilə faylın URL adresi təyin olunur:

```html
<video src="video.mp4" controls></video>
<audio src="audio.mp3" controls></audio>
```

Bundan əlavə brauzerlər fərqli fayl formatlarını dəstəkləyir. Video və səs fayllarının fərqli formatlarda olması üçün, faylın formatını təyin etmək üçün `type` atributu istifadə olunur:

```html
<video controls>
	<source src="video.mp4" type="video/mp4" />
	<source src="video.ogg" type="video/ogg" />
	Your browser does not support the video tag.
</video>
```

```html
<audio controls>
	<source src="audio.mp3" type="audio/mpeg" />
	<source src="audio.ogg" type="audio/ogg" />
	Your browser does not support the audio tag.
</audio>
```

`video` və `audio` elementlərinin ən vacib atributları aşağıdakılardır:

- `src`: Video və səs faylının URL adresini təyin edir.
- `controls`: Video və səs faylının naviqasiya düymələrini göstərir.
- `autoplay`: Video və səs faylını avtomatik başladar.
- `loop`: Video və səs faylını təkrar edir.
- `muted`: Video və səs faylının səsini söndərir.
- `preload`: Video və səs faylını yükləmək üçün təyin edir.

## Iframe

`<iframe>` elementi digər səhifəni ya da səhifə hissəsini göstərmək üçün istifadə olunur.

```html
<iframe src="https://www.w3schools.com"></iframe>
```

`src` atributu ilə göstərilən səhifəni göstərir. `width` və `height` atributları ilə ölçüləri təyin edilir.

```html
<iframe src="https://www.w3schools.com" width="400" height="400"></iframe>
```

Youtubedan iframe almaq üçün videoya sağ tıklayıb "Copy embed code" seçin və `<iframe>` elementini kopyalayın və ya paylaş hissəsindən "copy embed code" kopyalayıb yapışdırın.

## Tables

HTML-də cədvəllər `<table>` elementi ilə təyin olunur. Cədvəl başlıqları `<thead></thead>` təqləti arasında təyin olunur. Cədvəl sətrləri `<tr></tr>` təqləti arasında təyin olunur. `<thead></thead>` içindəki `<th></th>` elementləri cədvəl başlıqlarını təyin edir. Cədvəl məlumatları `<tbody></tbody>` içindəki `<td></td>` elementləri ilə təyin olunur. `<caption></caption>` elementi cədvələ başlıq əlavə etmək üçün istifadə olunur.

```html
<table>
	<caption>
		İşçilər
	</caption>
	<thead>
		<tr>
			<th>Ad</th>
			<th>Soyad</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Elvin</td>
			<td>Abdullayev</td>
		</tr>
		<tr>
			<td>Orxan</td>
			<td>Quliyev</td>
		</tr>
	</tbody>
</table>
```

`colspan` və `rowspan` atributları cədvəl sətrlərini və sütunlarını genişlətmək üçün istifadə olunur.

```html
<table>
	<tr>
		<td colspan="2">Ad Soyad</td>
	</tr>
	<tr>
		<td>Elvin</td>
		<td>Abdullayev</td>
	</tr>
</table>
```

## Semantic HTML

HTML-də semantic elementlər, səhifənin strukturu və məzmununu daha yaxşı anlamaq üçün istifadə olunur. Aşağıdakı semantic elementlər HTML-də istifadə olunur:

- `<header>`: Səhifənin başlığını təyin edir.
- `<nav>`: Səhifədəki naviqasiya hissəsini təyin edir.
- `<main>`: Səhifənin əsas məzmununu təyin edir.
- `<article>`: Səhifədəki məqalələri təyin edir.
- `<section>`: Səhifədəki bölmələri təyin edir.
- `<aside>`: Səhifədəki yan hissələri təyin edir.
- `<footer>`: Səhifənin alt hissəsini təyin edir.

Məntiq baxımından bir qutu rolunu oynayırlar və `<div>` elementlərinə nisbətən daha mənalıdırlar.

## div elementi

`<div>` elementi, HTML-də blok elementlərini qruplaşdırmaq üçün istifadə olunur və qutu rolunu oynayır. CSS və JavaScript ilə birlikdə istifadə olunur.

```html
<div style="background-color: lightblue;">
	<h1>HTML div elementi</h1>
	<p>
		HTML div elementi blok elementlərini qruplaşdırmaq üçün istifadə olunur.
	</p>
</div>
```

## CSS əlavə etmək

HTML-də CSS əlavə etmək üçün `<style>` elementi və ya `<link>` elementi istifadə olunur. `<style>` elementi səhifənin başlığında və ya səhifənin başlanğıcında təyin olunur (internal css). `<link>` elementi isə səhifənin başlığında təyin olunur(external css). Elementin içərisində `style` atributu ilə CSS təyin oluna bilir(inline css).

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    body {
      background-color: lightblue;
    }
    h1 {
      color: white;
      text-align: center;
    }
  </style>
</head>
<body>
  <h1>HTML CSS əlavə etmək</h1>
  <p>
    HTML-də CSS əlavə etmək üçün <style> elementi və ya <link> elementi istifadə olunur.
  </p>
</body>
</html>
```

```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
  <h1>HTML CSS əlavə etmək</h1>
  <p>
    HTML-də CSS əlavə etmək üçün <style> elementi və ya <link> elementi istifadə olunur.
  </p>
</body>
</html>
```

## Css sintaksisi

CSS-də seçicilər və təyinatlar istifadə olunur. Seçicilər HTML elementlərini seçmək üçün istifadə olunur. Təyinatlar isə seçilmiş elementlərə təyin olunur.

```css
body {
  background-color: lightblue;
}
h1 {
  color: white;
  text-align: center;
}
```

## class və id

HTML-də class və id atributları CSS təyin etmək üçün istifadə olunur. Class atributu bir neçə elementə eyni CSS təyin olunmasına imkan verir. Id atributu isə yalnız bir elementə CSS təyin olunmasına imkan verir.

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    .red {
      color: red;
    }
    #blue {
      color: blue;
    }
  </style>
</head>
<body>
  <h1 class="red">HTML class və id</h1>
  <p id="blue">
    HTML-də class və id atributları CSS təyin etmək üçün istifadə olunur.
  </p>
</body>
</html>
```

## CSS şərh sətirləri

CSS-də şərh sətirləri `/*` və `*/` arasında təyin olunur.

```css
/* Bu bir CSS şərh sətiri */
body {
  background-color: lightblue;
}
```

## CSS color

CSS-də rənglər `color` atributu ilə təyin olunur. Rənglər RGB, HEX və ya rəng adları ilə təyin oluna bilər.

```css
h1 {
  color: red;
}
h2{
  color: #ff0000;
}
h3{
  color: rgb(255, 0, 0);
}
```

## CSS font-size

CSS-də mətn ölçüsü `font-size` atributu ilə təyin olunur.

```css
h1 {
  font-size: 24px;
}
```