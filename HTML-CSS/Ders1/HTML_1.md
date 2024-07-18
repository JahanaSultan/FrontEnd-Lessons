# HTML Dərs 1

## HTML haqqında qısa məlumat

HTML (HyperText Markup Language), veb səhifələrinin strukturunu təyin edən bir işarələmə dilidir. HTML, veb səhifələrində mətn, şəkil, video, formalar və digər elementləri yerləşdirmək üçün istifadə olunur. HTML kodu, brauzerin səhifəni necə göstərməli olduğunu anlaması üçün etiketlər (tags) adlanan xüsusi elementlərdən ibarətdir. HTML5, ən son və ən genişləndirilmiş HTML versiyasıdır.

## HTML tarixi

HTML, 1993-cu ildə Tim Berners-Lee tərəfindən yaradılmışdır. HTML, 1995-ci ildə HTML 2.0 versiyası ilə standartlaşdırılmışdır. HTML, 1997-ci ildə HTML 4.0 versiyası ilə genişləndirilmişdir. HTML, 2008-ci ildə HTML 5.0 versiyası ilə yenilənmişdir. HTML5, 2014-cü ildə W3C tərəfindən standartlaşdırılmışdır.

## HTML etiketləri

HTML etiketləri, brauzerə səhifədəki məzmunun necə göstərilməli olduğunu bildirir. HTML etiketləri, açılış etiketi (`<tag>`) və bağlanış etiketi (`</tag>`) olmaqla iki hissədən ibarətdir. Açılış etiketi, etiketin nə zaman başladığını göstərir və bağlanış etiketi, etiketin nə zaman bitdiyini göstərir. Məsələn, mətni böyük şriftlə göstərmək üçün `<h1>` etiketi istifadə olunur.

## HTML sənədi yaradılması

HTML sənədi yaradmaq üçün, bir mətn redaktoru (notepad, notepad++, visual studio code, sublime text və s.) istifadə edə bilərsiniz. HTML sənədi, `.html` uzantılı fayl olmalıdır. Məsələn, `index.html` adlı bir fayl yaradaraq, HTML kodlarını bu faylın daxilinə yazaraq veb səhifə yarada bilərsiniz.

## HTML sənədində əsas elementlər

HTML sənədində əsas elementlər aşağıdakılardır:

- `<!DOCTYPE html>`: HTML sənədinin versiyasını göstərir.
- `<html>`: HTML sənədini başladır.
- `<head>`: Səhifənin başlığını və digər məlumatları daxil edir.
- `<title>`: Səhifənin başlığını təyin edir.
- `<body>`: Səhifənin əsas məzmununu daxil edir.
- `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`: Başlıqları təyin edir.
- `<p>`: Mətni təyin edir.
- `<a>`: Linkləri təyin edir.
- `<img>`: Şəkilləri təyin edir.
- `<ul>`, `<ol>`, `<li>`: Siyahıları təyin edir.
- `<table>`, `<tr>`, `<td>`, `<th>`: Cədvəlləri təyin edir.
- `<form>`, `<input>`, `<button>` və s.: Form elementlərini təyin edir.

## Format

Yazdığınız kodları daha gözəl və oxunaqlı etmək üçün, onları düzgün şəkildə formatlayın. HTML kodlarını formatlayarkən aşağıdakı qaydalara əməl edə bilərsiniz:

- Hər bir açılış etiketindən sonra yeni bir sətirə keçin.
- Açılış etiketlərini bağlanış etiketlərindən bir sətir aşağıda yazın.
- Bir tag daxilindəki məzmunu, iki boşluq (space) ilə indent edin.
- HTML sənədindəki əsas elementləri bir-birindən boşluqla ayırın.

Yazdığınız kodları avtomatik formatlamaq üçün bir mətn redaktoru istifadə edə bilərsiniz. Məsələn, Visual Studio Code mətn redaktoru, `Shift + Alt + F` kombinasiyasını vuraraq HTML kodlarını avtomatik formatlaya bilərsiniz.

## HTML elementləri

HTML elementləri, brauzerə məzmunun necə göstərilməli olduğunu bildirir. HTML elementləri, açılış etiketi, məzmun və bağlanış etiketi olmaqla üç hissədən ibarətdir:

```html
<tagname>Content buraya yazilacaq...</tagname>
```

İçərisinə kontent gəlməyən elementlərə **empty element** deyilir. Məsələn, `<img>` elementi. Bu elementlərə açılış etiketi ilə bağlanış etiketi arasında heç bir məzmun yazılmır və açılış etikeitindən sonra `/` işarəsi qoyulur:

```html
<img src="image.jpg" alt="Description" />
```

## HTML atributları

HTML atributları, elementlərə əlavə məlumatlar əlavə etmək üçün istifadə olunur. Atributlar, elementin davranışını və xüsusiyyətlərini təyin etmək üçün istifadə olunur. Atributlar, elementin açılış etiketində yazılır və `name="value"` formatında olur. Məsələn, `<img>` elementinə `src` və `alt` atributları əlavə edilə bilər. Ən çox istifadə olunan atributlar aşağıdakılardır:

- `id`: Elementə unikal bir ad təyin edir.
- `class`: Elementə bir və ya daha çox sinif adı təyin edir.
- `style`: Elementin CSS xüsusiyyətlərini təyin edir.
- `src`: Elementin məzmununu təyin edir.
- `href`: Elementin linkini təyin edir.
- `alt`: Elementin alternativ məzmununu təyin edir.
- `title`: Elementin başlığını təyin edir.
- `width`: Elementin genişliyini təyin edir.
- `height`: Elementin hündürlüyünü təyin edir.
- `colspan`: Cədvəl sütunlarını birləşdirir.
- `rowspan`: Cədvəl sətrlərini birləşdirir.
- `checked`: Checkbox və radio düymələrini işarələyir.
- `disabled`: Elementi deaktiv edir.
- `readonly`: Elementi yalnız oxuna bilən edir.
- `required`: Elementin doldurulması tələb olunur.
- `placeholder`: Elementə placeholder məzmununu təyin edir.
- `autocomplete`: Elementə avtomatik tamamlama funksiyasını təyin edir.
- `autofocus`: Elementə fokuslanır.
- `multiple`: Elementə birdən çox məzmun seçmə imkanı verir.
- `min`: Elementin minimum dəyərini təyin edir.
- `max`: Elementin maksimum dəyərini təyin edir.
- `step`: Elementin addımını təyin edir.
- `pattern`: Elementin daxilindəki məzmunun formatını təyin edir.
- `target`: Linkin açılacağı hədəf pencəsini təyin edir.
- `download`: Şəklin yüklənməsinə icazə verir.
- `rel`: Linkin məzmunu ilə bağlı məlumat verir.
- `type`: Input elementinin tipini təyin edir.
- `value`: Elementin dəyərini təyin edir.
- `name`: Elementin adını təyin edir.
- `for`: Label elementinin hədəfini təyin edir.
- `form`: Elementin mənəvi formunu təyin edir.
- `contenteditable`: Elementin məzmununu redaktə edilə bilən edir.

## HTML başlıqları

HTML başlıqları, səhifədəki məzmunun strukturunu təyin etmək üçün istifadə olunur. HTML başlıqları, `<h1>` ilə `<h6>` arasında dəyişir və məzmunun əhəmiyyət sırasına görə təyin edilir. Məsələn, `<h1>` başlığı ən əsas başlıq olaraq istifadə olunur və `<h6>` başlığı ən az əsasbaşlıq olaraq istifadə olunur. HTML başlıqları, məzmunu böyük şriftlə göstərmək üçün istifadə olunur:

```html
<h1>Bu bir h1 başlığıdır</h1>
<h2>Bu bir h2 başlığıdır</h2>
<h3>Bu bir h3 başlığıdır</h3>
<h4>Bu bir h4 başlığıdır</h4>
<h5>Bu bir h5 başlığıdır</h5>
<h6>Bu bir h6 başlığıdır</h6>
```

HTML də başlıq yazarkən mütləq başlıqın məzmununu `<h1>` ilə `<h6>` arasında yazın. Adi mətnləri böyük və qalın edərək başlıq kimi göstərməyin.

## HTML mətn elementləri

HTML mətn elementləri, səhifədəki mətni təyin etmək üçün istifadə olunur. HTML mətn elementləri, mətni böyük, kiçik, qalın, italik və digər xüsusiyyətlərlə göstərmək üçün istifadə olunur. Mətn elementləri aşağıdakılardır:

- `<p>`: Mətni təyin edir.
- `<ins>`: Mətni əlavə edilmiş kimi göstərir.
- `<q>`: Mətni təklif olaraq göstərir.
- `<blockquote>`: Mətni blok şəkildə göstərir.
- `<pre>`: Mətni öncədən formatlayaraq göstərir.
- `<code>`: Mətni proqram kodu kimi göstərir.
- `<kbd>`: Mətni klaviatura kombinasiyası kimi göstərir. Məsələn, `Ctrl + C`.
- `<samp>`: Mətni nümunə kimi göstərir.
- `<var>`: Mətni dəyişən kimi göstərir.
- `<abbr>`: Mətni qısaltma kimi göstərir.
- `<cite>`: Mətni istifadə olunan mənbə kimi göstərir.
- `<dfn>`: Mətni təyin edən mənayı göstərir.
- `<address>`: Mətni ünvan kimi göstərir.
- `details`: Mətni gizlətmək üçün istifadə olunur.
- `summary`: Gizlənmiş mətnin başlığını təyin edir.

## HTML Formatlama elementləri

HTML formatlama elementləri, səhifədəki mətni formatlamaq üçün istifadə olunur. HTML formatlama elementləri, mətni böyük, kiçik, qalın, italik və digər xüsusiyyətlərlə göstərmək üçün istifadə olunur. Formatlama elementləri aşağıdakılardır:

- `<b>`: Mətni qalın göstərir.
- `<strong>`: Mətni qalın göstərir.
- `<i>`: Mətni italik göstərir.
- `<em>`: Mətni italik göstərir.
- `<u>`: Mətni altıxətt göstərir.
- `<s>`: Mətni üstüxətt göstərir.
- `<sub>`: Mətni alt indeks kimi göstərir.
- `<sup>`: Mətni üst indeks kimi göstərir.
- `<small>`: Mətni kiçik şriftlə göstərir.
- `<hr>`: Qısa xətt əlavə edir.
- `<mark>`: Mətni işarələyir.
- `<del>`: Mətni silinmiş kimi göstərir.

## HTML şərh sətrləri

HTML şərh sətrləri, mətnin açıqlamasını və ya izahını əlavə etmək üçün istifadə olunur. HTML şərh sətrləri, brauzer tərəfindən oxunmur və yalnız mətn redaktoru tərəfindən görünür. HTML şərh sətrləri, `<!--` və `-->` işarələri arasında yazılır:

```html
<!-- Bu bir HTML şərh sətridir -->
```

HTML şərh sətrləri, mətn redaktoru tərəfindən kodun başqa proqramçılar tərəfindən daha asan anlaşılması üçün istifadə olunur. HTML şərh sətrləri, kodun hansı hissəsinin nə işlə yaradığını izah etmək üçün istifadə olunur. Kodu şərh sətrinə çevirmək üçün `Ctrl + /` kombinasiyasını vuraraq seçdiyiniz kodu şərh sətrinə çevirə bilərsiniz.

## HTML linkləri

HTML linkləri, səhifələr arasında keçidləri təyin etmək üçün istifadə olunur. HTML linkləri, `<a>` etiketi ilə təyin olunur və `href` atributu ilə hədəf səhifənin URL adresi təyin olunur. HTML linkləri, mətn və ya şəkil kimi elementlərə əlavə oluna bilər:

```html
<a href="https://www.example.com">Mətn linki</a>
<a href="https://www.example.com"><img src="image.jpg" alt="Description" /></a>
```

HTML linkləri, mətn və ya şəkil kimi elementlərə əlavə oluna bilər. Linklərə basdıqda hədəf səhifə açılır və istifadəçi hədəf səhifəyə yönləndirilir. Linklərə basdıqda hədəf səhifə yeni pəncərədə açılmasını istəyirsinizsə, `target="_blank"` atributunu əlavə edə bilərsiniz. Attributları aşağıdakılardır:

- `href`: Linkin hədəf səhifəsinin URL adresini təyin edir.
- `target`: Linkin açılacağı hədəf pencəsini təyin edir.
- `download`: Şəklin yüklənməsinə icazə verir.
- `rel`: Linkin məzmunu ilə bağlı məlumat verir.

## HTML şəkilləri

HTML şəkilləri, səhifədə şəkilləri və ya digər media fayllarını göstərmək üçün istifadə olunur. HTML şəkilləri, `<img>` etiketi ilə təyin olunur və `src` atributu ilə şəklin URL adresi təyin olunur. HTML şəkilləri, mətn və ya link kimi elementlərə əlavə oluna bilər:

```html
<img src="image.jpg" alt="Description" />
```

`img` elementinin ən vacib atributları aşağıdakılardır:

- `src`: Şəklin URL adresini təyin edir.
- `alt`: Şəklin alternativ məzmununu təyin edir.
- `width`: Şəklin genişliyini təyin edir.
- `height`: Şəklin hündürlüyünü təyin edir.
- `title`: Şəklin başlığını təyin edir.

## HTML siyahıları

HTML siyahıları, məlumatları qruplaşdırmaq və təşkil etmək üçün istifadə olunur. HTML siyahıları, `<ul>`, `<ol>` və `<li>` etiketləri ilə təyin olunur. HTML siyahıları, mətn, link və ya şəkil kimi elementlərə əlavə oluna bilər:

```html
<ul>
	<li>Element 1</li>
	<li>Element 2</li>
	<li>Element 3</li>
</ul>

<ol>
	<li>Element 1</li>
	<li>Element 2</li>
	<li>Element 3</li>
</ol>

<ul>
	<li><a href="https://www.example.com">Link 1</a></li>
	<li><a href="https://www.example.com">Link 2</a></li>
	<li><a href="https://www.example.com">Link 3</a></li>
</ul>

<ul>
	<li><img src="image1.jpg" alt="Description" /></li>
	<li><img src="image2.jpg" alt="Description" /></li>
	<li><img src="image3.jpg" alt="Description" /></li>
</ul>
```

HTML siyahıları, məlumatları qruplaşdırmaq və təşkil etmək üçün istifadə olunur. Siyahılar, mətn, link və ya şəkil kimi elementlərə əlavə oluna bilər. Siyahılar, `<ul>`, `<ol>` və `<li>` etiketləri ilə təyin olunur. `<ul>` etiketi, sırasız siyahıları təyin edir və `<ol>` etiketi, sıralı siyahıları təyin edir. `<li>` etiketi, siyahı elementlərini təyin edir.