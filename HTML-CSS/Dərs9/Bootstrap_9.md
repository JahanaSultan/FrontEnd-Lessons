# CSS Dərs 9

## Bootstrap

**Bootstrap** Twitter tərəfindən yaradılmış və hazırda geniş istifadə olunan açıq mənbə frontend frameworkudur. Bu framework mobil cihazlara uyğun, responsiv (müxtəlif ekran ölçülərinə uyğunlaşan) veb səhifələr yaratmağı asanlaşdırır. Bootstrap, HTML, CSS və JavaScript komponentlərindən ibarətdir.

### Bootstrap-ın Xüsusiyyətləri

1. **Responsiv Dizayn**: Bootstrap, müxtəlif cihazlarda (mobil telefonlar, planşetlər, kompüterlər) düzgün göstərilən veb səhifələr yaratmağa imkan verir.
2. **Komponentlər**: Bootstrap çoxlu sayda komponentlər (buttonlar, naviqasiya barları, modal pəncərələr və s.) təklif edir.
3. **Grid Sistemi**: Bootstrap-in grid sistemi (ızgara sistemi) müxtəlif ekran ölçülərinə uyğun olaraq məzmunu tənzimləməyə imkan verir.
4. **JavaScript Plugins**: Bootstrap, müxtəlif funksionallıqlar əlavə etmək üçün JavaScript plugins təklif edir (modal pəncərələr, alətlər, sürüşmə karuselləri və s.).

### Bootstrap-ın Tərkibi

1. **CSS Faylları**: Stil təyin etmək üçün lazım olan fayllar.
2. **JavaScript Faylları**: Dinamik funksiyaları təmin edən fayllar.
3. **İkonlar**: Bootstrap Icons vasitəsilə ikonlar əlavə etmək mümkündür.

### Bootstrap ilə Başlamaq

Bootstrap ilə başlamaq çox sadədir. Aşağıdakı addımları izləyərək ilk layihənizi qura bilərsiniz.

#### Addım 1: Bootstrap Fayllarını Layihəyə Daxil Etmək

Bootstrap-i iki yolla layihənizə daxil edə bilərsiniz: CDN (Content Delivery Network) vasitəsilə və ya lokal olaraq faylları yükləyərək.

**CDN Vasitəsilə:**

HTML faylınızın `<head>` bölməsinə aşağıdakı kodu əlavə edin:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bootstrap Layihəsi</title>
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <!-- Buraya məzmun gələcək -->
  <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.4/dist/umd/popper.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
```

**Lokal Fayllar:**

Bootstrap-in rəsmi saytından faylları yükləyin və layihənizin `css` və `js` qovluqlarına əlavə edin. Sonra bu fayllara HTML faylında istinad edin:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bootstrap Layihəsi</title>
  <link href="css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <!-- Buraya məzmun gələcək -->
  <script src="js/jquery-3.5.1.slim.min.js"></script>
  <script src="js/popper.min.js"></script>
  <script src="js/bootstrap.min.js"></script>
</body>
</html>
```

#### Addım 2: Grid Sistemindən İstifadə

Bootstrap-in grid sistemi, veb səhifənizin layoutunu tənzimləmək üçün istifadə olunur. Məsələn, üç sütunlu bir layout yaratmaq üçün aşağıdakı kodu istifadə edə bilərsiniz:

```html
<div class="container">
  <div class="row">
    <div class="col-md-4">Birinci Sütun</div>
    <div class="col-md-4">İkinci Sütun</div>
    <div class="col-md-4">Üçüncü Sütun</div>
  </div>
</div>
```

#### Addım 3: Komponentlərdən İstifadə

Bootstrap müxtəlif komponentlər təklif edir. Məsələn, düymələr (buttons) əlavə etmək üçün aşağıdakı kodu istifadə edə bilərsiniz:

```html
<button type="button" class="btn btn-primary">Əsas Düymə</button>
<button type="button" class="btn btn-secondary">İkinci Düymə</button>
<button type="button" class="btn btn-success">Uğur Düyməsi</button>
```

#### Addım 4: JavaScript Plugins

Məsələn, modal pəncərə əlavə etmək üçün aşağıdakı kodu istifadə edə bilərsiniz:

```html
<!-- Button trigger modal -->
<button type="button" class="btn btn-primary" data-toggle="modal" data-target="#exampleModal">
  Modal Aç
</button>

<!-- Modal -->
<div class="modal fade" id="exampleModal" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog" role="document">
    <div class="modal-content">
      <div class="modal-header">
        <h5 class="modal-title" id="exampleModalLabel">Modal başlığı</h5>
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
        Bu modalın məzmunudur.
      </div>
      <div class="modal-footer">
        <button type="button" class="btn btn-secondary" data-dismiss="modal">Bağla</button>
        <button type="button" class="btn btn-primary">Yadda saxla</button>
      </div>
    </div>
  </div>
</div>
```

### Nəticə

Bootstrap, veb dizaynını sadələşdirmək və sürətləndirmək üçün güclü bir vasitədir. Onun grid sistemi, komponentləri və JavaScript plugins-ləri ilə mürəkkəb və responsiv veb səhifələr yaratmaq mümkündür. Bootstrap-i öyrənmək, veb inkişafı sahəsində bacarıqlarınızı artırmaq üçün əla bir yoldur.

Bootstrap haqqında daha ətraflı məlumat üçün [rəsmi sənədlərə](https://getbootstrap.com/docs/5.0/getting-started/introduction/) müraciət edə bilərsiniz.