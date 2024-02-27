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
