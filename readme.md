JavaScript ma'lumotlarni turli yo'llar bilan "ko'rsatishi" mumkin:

dan foydalanib HTML elementiga yozish innerHTML.
dan foydalanib HTML chiqishiga yozish document.write().
dan foydalanib, ogohlantirish qutisiga yozish window.alert().
dan foydalanib brauzer konsoliga yozish console.log().

JavaScript o'zgaruvchisini e'lon qilishning 3 usuli:

1 - var
2 - let
3 - const

Functions
JavaScript funktsiyalari kalit so'z bilan aniqlanadifunction
Agar funktsiya etishmayotgan argumentlar bilan chaqirilsa (e'lon qilinganidan kamroq), etishmayotgan qiymatlar ga o'rnatiladi undefined.
JavaScript-da kalit so'z ob'ektgathis ishora qiladi
Boshqa funktsiyalar bilan parallel ravishda ishlaydigan funksiyalar asinxron deyiladi

```
function myDisplayer(something) {
  document.getElementById("demo").innerHTML = something;
}

function myCalculator(num1, num2, myCallback) {
  let sum = num1 + num2;
  myCallback(sum);
}

myCalculator(5, 5, myDisplayer);

```

Asynnc - bu boshqa funktsiyaga argument sifatida uzatiladigan funktsiya

Ushbu texnika funktsiyaga boshqa funktsiyani chaqirishga imkon beradi

Qayta qo'ng'iroq qilish funktsiyasi boshqa funktsiya tugagandan so'ng ishga tushishi mumkin
Object

JavaScript satrlari matnni saqlash va boshqarish uchun mo'ljallangan.

Xususiyat lengthsatr uzunligini qaytaradi:
Satrning bir qismini ajratib olishning 3 ta usuli mavjud:

slice(start, end)
substring(start, end)
substr(start, length)
slice()satrning bir qismini chiqaradi va chiqarilgan qismini yangi qatorga qaytaradi.
substring()ga o'xshaydi slice().

Farqi shundaki, 0 dan kichik boshlang'ich va yakuniy qiymatlar 0 sifatida qabul qilinadi substring().
Satr quyidagi bilan katta harfga aylantiriladi toUpperCase():
Satr quyidagi bilan kichik harfga aylantiriladi toLowerCase():
concat()ikki yoki undan ortiq qatorlarni birlashtiradi:
Usul trim()satrning ikkala tomonidagi bo'shliqni olib tashlaydi:

Array - bu bir nechta qiymatga ega bo'lishi mumkin bo'lgan maxsus o'zgaruvchi

JavaScript usuli toString()massivni (vergul bilan ajratilgan) massiv qiymatlari qatoriga aylantiradi.

pop()massivdan oxirgi elementni olib tashlaydi
push()massivga yangi element qo'shadi (oxirida):
shift()massivning birinchi elementini olib tashlaydi va qolgan barcha elementlarni pastki indeksga "o'tkazadi".
unshift()massivga yangi element qo'shadi (boshida) va eski elementlarni "o'chiradi":
concat()mavjud massivlarni birlashtirish (birlashtirish) orqali yangi massiv yaratadi:
Usul splice()massivga yangi elementlar qo'shadi.
Usul slice()massivning bir qismini ajratadi.

Switch
Loop
JSON - bu ma'lumotlarni saqlash va tashish uchun format

Dom

# 1. Meta teglar

Teg <meta>HTML hujjati haqidagi metama'lumotlarni belgilaydi. Metadata - bu ma'lumotlar haqidagi ma'lumotlar (ma'lumotlar).

<meta>teglar har doim <head> elementi ichiga kiradi va odatda belgilar to'plamini, sahifa tavsifini, kalit so'zlarni, hujjat muallifini va ko'rish oynasi sozlamalarini belgilash uchun ishlatiladi.

Metadata sahifada ko'rsatilmaydi, lekin mashinada tahlil qilinadi.

Metadata brauzerlar (tarkibni qanday ko'rsatish yoki sahifani qayta yuklash), qidiruv tizimlari (kalit so'zlar) va boshqa veb-xizmatlar tomonidan qo'llaniladi.

Veb-dizaynerlarga teg orqali ko'rish oynasini (veb-sahifaning foydalanuvchining ko'rinadigan maydoni) nazorat qilish imkonini beradigan usul mavjud <meta>(quyidagi "Ko'rish portini o'rnatish" misoliga qarang).

# 2. pesudo class va pseudo element farqi?

Pseudo-sinflar va psevdoelementlar - bu CSS xususiyatlari bo'lib, ular sizga hujjatdagi muayyan elementlarni uslublash uchun yo'naltirish imkonini beradi. Biroq, ular turli maqsadlarga xizmat qiladi va ba'zi asosiy farqlarga ega:

Psevdo-sinflar:
Pseudo-klasslar elementning maxsus holatini aniqlash uchun ishlatiladi. Masalan, :hover foydalanuvchi kursorni uning ustiga olib borganida elementni nishonga oladi.
Pseudo-sinflar oldida ikki nuqta qo'yiladi: CSS da.
Ular foydalanuvchi shovqini yoki dinamik holatlarga asoslangan elementlarni uslublash uchun ishlatiladi, masalan :hover , :active , :focus , :first-child va boshqalar.
Pseudo-sinflar element selektoridan keyin yoziladi, masalan a:hover langar elementlarining hover holatini nishonga oladi.
Psevdo elementlar:
Pseudo-elementlar hujjat daraxtida asl HTMLda mavjud bo'lmagan qo'shimcha elementlarni yaratishga imkon beradi. Masalan, :: oldin va :: keyin.
CSS-da psevdo-elementlar oldidan ikkita nuqta :: qo'yiladi.
Ular elementning muayyan qismlarini uslublash yoki elementdan oldin yoki keyin tarkibni kiritish uchun ishlatiladi.
Pseudo-elementlar selektordan va CSS qoidasidagi har qanday psevdo-sinflardan keyin kelishi kerak. Masalan, p::birinchi qator <p> elementining birinchi qatoriga mo'ljallangan.
Asosiy farqlar:
Maqsad: Pseudo-sinflar foydalanuvchining oʻzaro taʼsiri yoki dinamik oʻzgarishlarga asoslangan elementning oʻziga xos holatini nishonga oladi, psevdoelementlar esa elementning alohida qismlari yoki qoʻshimcha tarkibni nishonga oladi.

Sintaksis: Pseudo-sinflar bitta ikki nuqtadan foydalanadilar: psevdo-elementlar esa ikki nuqtadan foydalanadilar ::.

Ilova: Pseudo-sinflar :hover yoki :focus kabi holatlarga asoslangan uslublarni qo'llash uchun, psevdo-elementlar esa qo'shimcha tarkib yaratish yoki elementning muayyan qismlarini uslublash uchun ishlatiladi.

Xulosa qilib aytadigan bo'lsak, psevdo-sinflar holat yoki foydalanuvchi o'zaro ta'siriga asoslangan uslublar uchun ishlatiladi, psevdo-elementlar esa qo'shimcha elementlarni kiritish yoki elementning muayyan qismlarini uslublash uchun ishlatiladi. Ikkala xususiyat ham boy va interaktiv veb-dizaynlarni yaratish uchun muhimdir.

# 3. Ta'rif: Sassdagi mixin - bu qayta ishlatilishi va boshqa uslublarga kiritilishi mumkin bo'lgan uslublar blokidir.

Foydalanish: Mixinlar turli elementlar yoki selektorlarda takrorlanadigan uslublarni birlashtirish uchun ishlatiladi.
Sintaksis: Miksinlar @mixin va keyin nom bilan belgilanadi va argumentlarni qabul qilishi mumkin. Ular @include yordamida kiritilgan.
Misol:
@mixin button-styles($color) {
fon rangi: $color;
to'ldirish: 10px;
chegara: 1px qattiq $color;
}

tugma {
@include tugma uslublari(qizil);
}

---

Kengaytirish:
Ta'rif: Sassda kengaytirish - bu xususiyatlar to'plamini bir selektordan ikkinchisiga almashish usuli.
Foydalanish: Extend bir selektorning uslublarini boshqasiga kengaytirish orqali uslublarning takrorlanmasligi uchun ishlatiladi.
Sintaksis: Kengaytmalar % va keyin nom bilan belgilanadi va @extend bilan ishlatiladi.
Misol:
%button-uslublari {
fon rangi: ko'k;
to'ldirish: 10px;
chegara: 1px to'liq ko'k;
}

tugma {
@extend %button-uslublari;
}
Asosiy farqlar:
Qayta ishlatmoq:

Miksinlar argumentlarni o'tkazish qobiliyatiga ega bo'lgan boshqa selektorlarga qo'shish orqali uslublar blokini qayta ishlatishga imkon beradi.
Extend mavjud uslublarni bir selektordan ikkinchisiga almashish uchun ishlatiladi, bu takrorlashni kamaytiradi.
Yaratilgan CSS:

Miksinlar ular kiritilgan har bir joy uchun takroriy CSS chiqishiga olib keladi.
Extend barcha kengaytirilgan selektorlar o'rtasida taqsimlanadigan yagona CSS qoidasini yaratadi, bu esa chiqish hajmini kamaytiradi.
Argumentlar:

Miksinlar argumentlarni qabul qilishi mumkin, bu ularni dinamik uslublarni yaratish uchun ko'p qirrali qiladi.
Extend argumentlarni uzatishni qo'llab-quvvatlamaydi.
Qo'llash doirasi:

Miksinlar qaerga qo'shilishidan qat'iy nazar kiritiladigan inkapsullangan uslublarni yaratadi.
Extend selektorlar o'rtasida munosabatlarni yaratadi, bu erda bir selektordagi uslublar boshqasiga qo'llaniladi.
Xulosa qilib aytganda, mixinlar argumentlar bilan qayta ishlatilishi mumkin bo'lgan uslub bloklari uchun ishlatiladi, kengaytirilganlar esa yaratilgan CSS chiqishidagi ortiqchalikni kamaytirish uchun selektorlar o'rtasida uslub xususiyatlarini almashish uchun ishlatiladi. Ikkalasi ham Sass uslublar jadvalida kuchli vositalar bo'lishi mumkin va ular orasidan tanlash loyihaning o'ziga xos talablariga bog'liq.

# 4 .JavaScript ma'lumotlar turlari:

JavaScript-da o'zgaruvchi ushlab turishi mumkin bo'lgan qiymatlar turini belgilaydigan bir nechta ma'lumotlar turlari mavjud. JavaScript-da keng tarqalgan ma'lumotlar turlari:

Primitiv ma'lumotlar turlari:

Raqam: Raqamli qiymatlarni ifodalaydi. U butun sonlarni, floatlarni va NaN va Infinity kabi maxsus raqamli qiymatlarni o'z ichiga oladi.
String: bitta yoki ikkita tirnoq ichiga olingan matnli ma'lumotlarni ifodalaydi.
Mantiqiy: mantiqiy qiymatni ifodalaydi - true yoki false .
Null: har qanday qiymatning qasddan yo'qligini ifodalaydi.
Aniqlanmagan: e'lon qilingan, lekin qiymat tayinlanmagan o'zgaruvchini ifodalaydi.
Belgi (ES6): Ob'ekt xususiyatlari uchun identifikator sifatida ishlatiladigan noyob va o'zgarmas qiymatni ifodalaydi.
Kompozit ma'lumotlar turlari:

Ob'ekt: Kalitlar (xususiyatlar/usullar) bilan aniqlangan kalit-qiymat juftliklari to'plamini ifodalaydi.
Massiv: Indekslar tomonidan foydalaniladigan elementlarning ro'yxatga o'xshash to'plamini ifodalaydi.
Funktsiya: chaqiriladigan funksiyani ifodalaydi.
Maxsus ma'lumotlar turlari:

BigInt (ES11): Katta butun sonlarni ixtiyoriy aniqlik bilan ifodalaydi.
Nullish Coalescing Operator ma'lumotlar turlari (ES11): null va undefined .
Ma'lumotnomalar (ma'lumotlar bo'lmagan turlari):

Funktsiya
Ob'ekt
Eslatma uchun muhim:
JavaScript dinamik ravishda terilgan til bo'lib, o'zgaruvchilar ma'lum bir ma'lumot turiga bog'lanmaydi.
Qiymatlar kontekstga asoslangan holda bir ma'lumot turidan boshqasiga dinamik ravishda o'zgartirilishi mumkin (Type majburlash).
Ma'lumotlar turlarini tushunish samarali va xatosiz JavaScript kodini yozish uchun juda muhimdir.
JavaScript-da turli xil ma'lumotlar turlarini tushunish mustahkam va samarali kod yozish, ma'lumotlarni to'g'ri ishlash va turlarni o'zgartirish va taqqoslash bilan bog'liq umumiy tuzoqlardan qochish uchun juda muhimdir.

JavaScript ma'lumotlar turlari:
JavaScript-da o'zgaruvchi ushlab turishi mumkin bo'lgan qiymatlar turini belgilaydigan bir nechta ma'lumotlar turlari mavjud. JavaScript-da keng tarqalgan ma'lumotlar turlari:

Primitiv ma'lumotlar turlari:

Raqam: Raqamli qiymatlarni ifodalaydi. U butun sonlarni, floatlarni va NaN va Infinity kabi maxsus raqamli qiymatlarni o'z ichiga oladi.
String: bitta yoki ikkita tirnoq ichiga olingan matnli ma'lumotlarni ifodalaydi.
Mantiqiy: mantiqiy qiymatni ifodalaydi - true yoki false .
Null: har qanday qiymatning qasddan yo'qligini ifodalaydi.
Aniqlanmagan: e'lon qilingan, lekin qiymat tayinlanmagan o'zgaruvchini ifodalaydi.
Belgi (ES6): Ob'ekt xususiyatlari uchun identifikator sifatida ishlatiladigan noyob va o'zgarmas qiymatni ifodalaydi.
Kompozit ma'lumotlar turlari:

Ob'ekt: Kalitlar (xususiyatlar/usullar) bilan aniqlangan kalit-qiymat juftliklari to'plamini ifodalaydi.
Massiv: Indekslar tomonidan foydalaniladigan elementlarning ro'yxatga o'xshash to'plamini ifodalaydi.
Funktsiya: chaqiriladigan funksiyani ifodalaydi.
Maxsus ma'lumotlar turlari:

BigInt (ES11): Katta butun sonlarni ixtiyoriy aniqlik bilan ifodalaydi.
Nullish Coalescing Operator ma'lumotlar turlari (ES11): null va undefined .
Ma'lumotnomalar (ma'lumotlar bo'lmagan turlari):

Funktsiya
Ob'ekt
Eslatma uchun muhim:
JavaScript dinamik ravishda terilgan til bo'lib, o'zgaruvchilar ma'lum bir ma'lumot turiga bog'lanmaydi.
Qiymatlar kontekstga asoslangan holda bir ma'lumot turidan boshqasiga dinamik ravishda o'zgartirilishi mumkin (Type majburlash).
Ma'lumotlar turlarini tushunish samarali va xatosiz JavaScript kodini yozish uchun juda muhimdir.
JavaScript-da turli xil ma'lumotlar turlarini tushunish mustahkam va samarali kod yozish, ma'lumotlarni to'g'ri ishlash va turlarni o'zgartirish va taqqoslash bilan bog'liq umumiy tuzoqlardan qochish uchun juda muhimdir.

# 5 variables difference ?

JavaScript-dagi o'zgaruvchilar:
JavaScript-dagi o'zgaruvchilar ma'lumotlarni saqlash va boshqarish uchun ishlatiladi. JavaScript-da turli xil turdagi o'zgaruvchilar o'rtasidagi ba'zi asosiy farqlar:

Var:

Var funksiya doirasiga ega.
var bilan e'lon qilingan o'zgaruvchilar o'z funksiyalari yoki global qamrovining yuqori qismiga ko'tariladi.
Var qayta tayinlanishi va qayta e'lon qilinishi mumkin.
Var deklaratsiyasi bloklangan emas.
Keling:

Keling, bloklangan. U aniqlangan blok (bayonot yoki ifoda) bilan chegaralanadi.
Let bilan e'lon qilingan o'zgaruvchilar blokning yuqori qismiga ko'tarilmaydi.
Keling, qayta tayinlanishi mumkin, lekin bir xil blok doirasida qayta e'lon qilinmaydi.
Const:

Const blok-ko'lamli.
const bilan e'lon qilingan o'zgaruvchilar deklaratsiya vaqtida ishga tushirilishi kerak va ularni qayta tayinlab bo'lmaydi.
Const o'zgaruvchilari blokning yuqori qismiga ko'tarilmaydi.
Const o'zgarmaslikni anglatmaydi. Agar const o'zgaruvchisi ob'ektga havolaga ega bo'lsa, ob'ektning xususiyatlarini o'zgartirish mumkin.
Asosiy farqlar:
Qo'llanish doirasi: Var funksiya doirasi, Let va Const esa blokli.
Yuk ko'tarish: Var deklaratsiyasi o'z funksiyasi yoki global miqyosning yuqori qismiga ko'tariladi, Let va Const esa ko'tariladi, lekin ishga tushirilmaydi.
Qayta tayinlash: Var va Let o'zgaruvchilari qayta tayinlanishi mumkin, lekin Const o'zgaruvchilari ishga tushirilgandan keyin qayta tayinlanmaydi.
Qayta deklaratsiya: Var xuddi shu miqyosda qayta deklaratsiya qilishga ruxsat beradi, lekin Let ruxsat bermaydi.
O'zgaruvchanlik: Const o'zgaruvchilari ob'ektlar uchun o'zgarmas emas. O'zgaruvchining o'zi doimiy, lekin ob'ekt xususiyatlarini o'zgartirish mumkin.
Ushbu farqlarni tushunish tuzilgan va xatosiz JavaScript kodini yozish uchun juda muhim, bu o'zgaruvchan xatti-harakatlarning kerakli hajm va o'zgaruvchanlik talablariga mos kelishini ta'minlaydi.

# 6. Number methods

JavaScript-da raqamlash usullari:
JavaScript-da Number ob'ekti raqamli ma'lumotlar turini ifodalovchi global ob'ektdir. U raqamlar ustida turli operatsiyalarni bajarishga imkon beruvchi bir nechta foydali usullar bilan birga keladi. Mana bir nechta umumiy raqam usullari:

toFixed():

Raqamni satrga aylantiradi va raqamni belgilangan kasr soniga yaxlitlaydi.
Sintaksis: number.toFixed(decimalPlaces)
toString():

Raqamni satrga aylantiradi.
Sintaksis: raqam.toString(asosiy)
toExponential():

Eksponensial belgida raqamni ifodalovchi qatorni qaytaradi.
Sintaksis: raqam.toExponential(fractionDigits)
toPrecision():

Belgilangan aniqlikdagi raqamni ifodalovchi qatorni qaytaradi.
Sintaksis: raqam.toPrecision(aniqlik)
parseInt():

Satrni tahlil qiladi va butun sonni qaytaradi.
Sintaksis: parseInt (string, radix)
parseFloat():

Satrni tahlil qiladi va suzuvchi nuqtali raqamni qaytaradi.
Sintaksis: parseFloat (string)
isNaN():

Qiymat NaN (Not-A-Number) ekanligini aniqlaydi.
Sintaksis: Number.isNaN(qiymat)
isFinite():

Qiymat chekli son ekanligini aniqlaydi.
Sintaksis: Number.isFinite(qiymat)
isInteger():

Raqam butun son ekanligini aniqlaydi.
Sintaksis: Number.isInteger(qiymat)
isSafeInteger():

Raqam xavfsiz butun son ekanligini aniqlaydi.
Sintaksis: Number.isSafeInteger(qiymat)
Bu usullar JavaScript-da raqamlar bilan ishlash uchun raqamlarni turli formatlarga aylantirish, ma'lum raqamlar turlarini tekshirish va raqamlar bilan bog'liq operatsiyalarni bajarish kabi bir qator funktsiyalarni ta'minlaydi. Ushbu usullar bilan tanishish JavaScript kodingizda raqamlarni samarali boshqarish va boshqarishga yordam beradi.

# 7 . Math method

JavaScript-dagi Math ob'ekti o'rnatilgan ob'ekt bo'lib, matematik hisoblar uchun matematik doimiylar va funktsiyalarni ta'minlaydi. Math ob'ektining ba'zi usullari va xususiyatlariga quyidagilar kiradi:

- Math.PI: Aylana aylanasining diametriga nisbatini ifodalovchi xususiyat, taxminan 3,14159.
- Math.sqrt(x): Sonning kvadrat ildizini qaytaruvchi usul.
- Math.pow(x, y): x ning y darajasiga ko'tarilgan qiymatini qaytaruvchi usul.
- Math.random(): 0 dan 1 gacha bo'lgan psevdo-tasodifiy raqamni qaytaradigan usul.
- Math.floor(x): Berilgan sondan kichik yoki unga teng eng katta butun sonni qaytaruvchi usul.
- Math.ceil(x): Berilgan sondan katta yoki unga teng eng kichik butun sonni qaytaruvchi usul.

Bu JavaScript-dagi Math ob'ekti tomonidan taqdim etilgan ko'plab matematik funktsiyalar va doimiylarning bir nechta misollari.

# 8. String method

1. length() - satr uzunligini qaytaradi.
2. toUpperCase() - satrni bosh harfga o'zgartiradi.
3. toLowerCase() - satrni kichik harfga o'zgartiradi.
4. indexOf() - satrda belgilangan qiymatning birinchi marta paydo bo'lishi indeksini qaytaradi.
5. lastIndexOf() - satrda belgilangan qiymatning oxirgi takrorlanish indeksini qaytaradi.
6. charAt() - satrda belgilangan indeksdagi belgini qaytaradi.
7. concat() - ikki yoki undan ortiq satrlarni birlashtiradi va yangi qatorni qaytaradi.
8. slice() - satrning bir qismini chiqaradi va yangi qatorni qaytaradi.
9. substr() - belgilangan indeksdan boshlab satrdan belgilangan miqdordagi belgilarni ajratib oladi va yangi qatorni qaytaradi.
10. replace() - belgilangan qiymatni satrdagi boshqa qiymat bilan almashtiradi.
11. split() - belgilangan ajratuvchiga asoslangan qatorni pastki qatorlar qatoriga ajratadi.
12. trim() - satrning ikkala uchidagi oq bo'shliqni olib tashlaydi.
13. match() - belgilangan qiymat uchun satrni qidiradi va topilgan qiymatni qaytaradi.
14. search() - Belgilangan qiymat uchun satrni qidiradi va mos keladigan joyni qaytaradi.

# 9. Undefined vs null ?

JavaScript-da "Undefined" va "null" ikkalasi ham qiymat yo'qligini ifodalash uchun ishlatiladi, ammo ular biroz boshqacha ma'noga ega:

- `Undefined` - ishga tushirilmagan o'zgaruvchiga yoki ob'ektda mavjud bo'lmagan xususiyatga tayinlangan ibtidoiy qiymat. Bu qiymat ataylab o'rnatilmaganligini bildiradi.
- `null` ham qiymatning qasddan yo`qligini ifodalovchi ibtidoiy qiymatdir. Odatda o'zgaruvchi yoki xususiyatning qiymati yo'qligini aniq ko'rsatish uchun ishlatiladi.

Umuman olganda, o'zgaruvchi yoki xususiyatni hech qanday qiymatga ega bo'lmagan holda aniq belgilashni maqsad qilganingizda "null" dan foydalanish tavsiya etiladi, "Undefined" esa qiymat o'rnatilmagan yoki mavjud emasligini ko'rsatish uchun ishlatiladi.

# 10.

JavaScript-da truthy , va falthy qiymatlar mantiqiy baholash bilan bog'liq tushunchalardir. JavaScript-dagi har bir qiymat o'ziga xos boolean "truthy ," yoki "falthy " ga ega, ya'ni ular mantiqiy kontekstlarda, masalan, shartli bayonotlar yoki mantiqiy operatsiyalarda to'g'ri yoki noto'g'ri baholanishi mumkin.

truthy ,: Agar mantiqiy qiymatga majburlanganda u truthy , deb baholansa, qiymat truthy , deb hisoblanadi. truthy , qiymatlarga misollar bo'sh bo'lmagan satrlar, 0 dan boshqa raqamlar, massivlar, ob'ektlar va funktsiyalarni o'z ichiga oladi.

falthy qiymatlar: to'g'ri bo'lmagan qiymatlar falthy qiymatlar deb hisoblanadi. 0, null, undefined, NaN, false (mantiqiy qiymat) va bo'sh qator ("").
