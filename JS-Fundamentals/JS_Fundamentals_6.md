# Javascript Dərs 6

## Javascript class-lar və OOP

Obyektyönümlü proqramlaşdırma, proqramları obyektlərdən istifadə edərək yazmaq deməkdir. Obyektlər, real həyatda gördüyümüz şeylər kimi düşünülə bilər. Məsələn, bir maşın, bir quş, ya da bir kompüter. Hər bir obyektin xüsusiyyətləri (properties) və hərəkətləri (methods) var.

**Nümunə:**

- **Maşın** bir obyektdir.
  - **Xüsusiyyətləri**: rəngi, markası, modeli
  - **Hərəkətləri**: sürmək, dayandırmaq

Class, obyektlər yaratmaq üçün bir şablondur. Elə bil ki, bir maşın yaratmaq üçün bir reseptdir. Class, necə obyektlər yaradılacağını və bu obyektlərin hansı xüsusiyyətlərə və hərəkətlərə malik olacağını müəyyən edir.

JavaScript-də bir class yaratmaq üçün `class` sözündən istifadə edirik. Aşağıda sadə bir maşın class-ı nümunə olaraq göstərilib:

```javascript
class Masin {
  constructor(reng, marka, model) {
    this.reng = reng;
    this.marka = marka;
    this.model = model;
  }

  sur() {
    console.log(`${this.marka} ${this.model} sürülür!`);
  }

  dayandir() {
    console.log(`${this.marka} ${this.model} dayandırıldı!`);
  }
}
```

Burada:
- `constructor` maşının rəngi, markası və modeli kimi xüsusiyyətləri təyin edir.
- `sur` və `dayandir` isə maşının hərəkətləridir.

Class-dan istifadə edərək obyekt yaratmaq üçün `new` sözündən istifadə edirik. Aşağıda iki maşın obyekti yaradılır:

```javascript
let masin1 = new Masin('qara', 'BMW', 'X5');
let masin2 = new Masin('ağ', 'Audi', 'A6');
```

Bu maşınlar yaradıldıqdan sonra onların hərəkətlərini çağıra bilərik:

```javascript
masin1.sur(); // BMW X5 sürülür!
masin2.dayandir(); // Audi A6 dayandırıldı!
```

OOP, kodları daha təşkilatlı və təkrar istifadəyə yararlı edir. Məsələn, fərqli maşın modelləri yaratmaq üçün hər dəfə eyni kodu yazmağa ehtiyac yoxdur. Yalnız bir class yaradıb, ondan istifadə edərək çoxlu maşın yarada bilərik.

- **Obyektlər** real həyatda gördüyümüz şeylər kimidir, xüsusiyyətləri və hərəkətləri var.
- **Class** obyektlər yaratmaq üçün bir şablondur.
- **Obyektyönümlü proqramlaşdırma** kodu daha təşkilatlı və təkrar istifadəyə yararlı edir.


## JSON 

JSON, məlumatları saxlamaq və ötürmək üçün istifadə olunan sadə bir formatdır. Adı üzərində, JavaScript obyektlərinin formatına bənzəyir, lakin demək olar ki, bütün proqramlaşdırma dilləri ilə istifadə edilə bilər. JSON, məlumatları oxumaq və yazmaq üçün asan olan strukturlaşdırılmış bir yol təklif edir.

### JSON Necə Görünür?

JSON, əsasən açar-dəyər cütlüklərindən ibarət olan bir mətn formatıdır. Hər bir açarın dəyəri ola bilər: ədəd, mətn (string), obyekt, siyahı (array), doğru/yanlış (boolean) və ya boş (null). Aşağıda sadə bir JSON nümunəsi var:

```json
{
  "ad": "Ali",
  "yas": 25,
  "evli": false,
  "uşaqlar": [
    {
      "ad": "Ayşe",
      "yas": 5
    },
    {
      "ad": "Mehmet",
      "yas": 3
    }
  ],
  "adres": {
    "şəhər": "Bakı",
    "ölkə": "Azərbaycan"
  }
}
```

Burada:
- `"ad"`, `"yas"`, `"evli"` açarlardır.
- `"Ali"`, `25`, `false` bu açarların dəyərləridir.
- `"uşaqlar"` açarı bir siyahıdır, içində iki obyekt var.
- `"adres"` açarı başqa bir obyektdir.

### JSON Nə Üçün İstifadə Olunur?

1. **Məlumat Mübadiləsi**: Veb brauzer ilə server arasında məlumat mübadiləsi üçün geniş istifadə olunur. Məsələn, bir veb səhifəsi serverdən istifadəçi məlumatlarını almaq istədikdə, server bu məlumatları JSON formatında göndərə bilər.

2. **Məlumat Saxlanması**: Kiçik həcmli məlumatları saxlamaq üçün istifadə edilə bilər. JSON faylları, məlumatların saxlanması və ötürülməsi üçün çox əlverişlidir.

3. **Konfiqurasiya Faylları**: Proqramların və tətbiqlərin konfiqurasiya məlumatlarını saxlamaq üçün JSON faylları geniş istifadə olunur.

### JavaScript-də JSON ilə İşləmək

JavaScript-də JSON formatında məlumatları oxumaq və yazmaq çox asandır.

#### JSON Məlumatlarını JavaScript Obyektinə Çevirmək

```javascript
let jsonMetni = '{"ad": "Ali", "yas": 25, "evli": false}';
let obyekt = JSON.parse(jsonMetni);

console.log(obyekt.ad); // Ali
console.log(obyekt.yas); // 25
console.log(obyekt.evli); // false
```

#### JavaScript Obyektini JSON Məlumatlarına Çevirmək

```javascript
let obyekt = { ad: "Ali", yas: 25, evli: false };
let jsonMetni = JSON.stringify(obyekt);

console.log(jsonMetni); // {"ad":"Ali","yas":25,"evli":false}
```

### Xülasə

- **JSON**: Məlumatları saxlamaq və ötürmək üçün istifadə olunan sadə bir mətn formatıdır.
- **İstifadə Məqsədləri**: Məlumat mübadiləsi, məlumat saxlanması, konfiqurasiya faylları.
- **JavaScript-də JSON**: JSON.parse() və JSON.stringify() metodları ilə JSON məlumatlarını asanlıqla idarə edə bilərik.

# Dərs 6 Tapşırıqlar

1. Aşağıdakı class-ı tərtib edin:

```javascript
class Kitab {
  constructor(ad, müəllif, say) {
    this.ad = ad;
    this.müəllif = müəllif;
    this.say = say;
  }

  təsvir() {
    console.log(`${this.ad} kitabı ${this.müəllif} tərəfindən yazılıb.`);
  }
}
```

2. Yuxarıdakı class-dan istifadə edərək iki kitab obyekti yaradın və onların təsvirini yazdırın.

3. Aşağıdakı JSON məlumatını JavaScript obyektinə çevirin və məlumatları yazdırın:

```json
{
  "ad": "Ali",
  "yas": 25,
  "evli": false,
  "uşaqlar": [
    {
      "ad": "Ayşe",
      "yas": 5
    },
    {
      "ad": "Mehmet",
      "yas": 3
    }
  ],
  "adres": {
    "şəhər": "Bakı",
    "ölkə": "Azərbaycan"
  }
}
```

4. Aşağıdakı JavaScript obyektini JSON məlumatına çevirin:

```javascript
let obyekt = { ad: "Ali", yas: 25, evli: false };
```