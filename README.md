# e-imzo
<b><a href="https://ubuntu.com/">Ubuntu</a></b> uchun mo'ljallangan <b><a href="https://e-imzo.uz/">E-IMZO</a></b> modulining paket ko'rinishidagi versiyasi

Assalomu alaykum! Avvalombor repozitoriyamga xush kelibsiz!

Bu versiyani yasashdan maqsad, kelajakda ish joyimda linuxga o'tish ehtiyoji mavjudligi uchun yengillik yaratdim.
Repozitoriyani yangilab boraman deb va'da bera olmayman, ammo vaqt bo'lganida yangiliklardan qolib ketmaslik uchun kuzatib turaman.

# paketni yig'ish qo'llanmasi
1) Oldin repozitoriyadan loyihani o'zingizga yuklab oling: 
<code>git clone https://github.com/SignalMQ/e-imzo.git</code>
2) Keyin <code>e-imzo</code> papkasi turgan direktoriyaga o'ting (lekin ichkariga o'tmang)
3) Ubuntu terminalini shu direktoriyada oching va quyidagi buyruqni tering: 
<code>dpkg-deb --build ./e-imzo</code>
4) Tayyor bo'lishini kuting va shu direktoriyada <code>.deb</code> paketni ko'rasiz:
![Screenshot from 2023-09-30 19-24-45](https://github.com/SignalMQ/e-imzo/assets/77734001/51d381c9-3349-4b10-b926-4fe446a69e8a)
# paketni o'rnatish
1) Tayyor bo'lgan paketni o'rnatish uchun quyidagi buyruqni tering: <code>sudo apt install ./e-imzo.deb</code>
2) Paket menejeri modul uchun kerakli bo'lgan yana boshqa paketlarni ham ko'rsatadi:
![Screenshot from 2023-09-30 19-32-51](https://github.com/SignalMQ/e-imzo/assets/77734001/c26e2c1f-20d4-4b48-89a8-ba603fa7c878)
3) <code>y</code> ni tering va <code>Enter</code> tugmasini bosing
4) O'rnatilish jarayoni tugagandan so'ng kompyuteringizni o'chirib yoqing
# duch kelishingiz mumkin bo'lgan muammolar
Agarda sizda shunday muammo paydo bo'lgan bo'lsa:
![Снимок экрана от 2023-11-04 16-09-51](https://github.com/SignalMQ/e-imzo/assets/77734001/671de0a3-e350-4b79-a7fd-3799c7d901b4)<br>
<b>Buning yechimi quyidagiday:</b>
1) <code>cd ./e-imzo/DEBIAN/</code>
2) <code>chmod 0775 control postinst prerm</code>
![Снимок экрана от 2023-11-04 16-16-25](https://github.com/SignalMQ/e-imzo/assets/77734001/17db0a5b-0c59-4c45-86bb-e23f0236a844)<br>
va natijada <code>dpkg-deb --build ./e-imzo</code> o'xshashi kerak:
![Снимок экрана от 2023-11-04 16-22-23](https://github.com/SignalMQ/e-imzo/assets/77734001/17c380c0-616b-4c1c-ac11-aff8f1509dba)
