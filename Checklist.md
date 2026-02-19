# Kapital Bank  Veb  Tətbiqi - TEST  CHECKLİST
 ## LOGİN / Autentifikasiya
- ###  Duzgün  istifadəçi  adı  və  parol  ilə  tətbiqə   giriş  mümkündür
-  ### Yanlış  şifrə  daxil  edildikdə  xəta  mesajı  görünür
- ###  Login  sahələri  boş  olduqda   girişə  icazə  verilmir
- ###  Şifrəni  unutdum linki  düzgün  işləyir
- ### Ç+Şifrə  qısa olduqda yəni  minimum  8 simvol limitindən  az olduqda error  mesajı çıxır
- ### Şifrə  çox uzun olduqda error  mesajı  və ya limit  tətbiq  olunur
- ### Şifrədə  böyük  və  kiçik  hərflərin eyni  zamanda  xüsüsi   simvolların    istifadəsinə  icazə  verilir
-  ### Login  sətrində  şifrə  maskalanır
-  ### Bir neçə  səhv  cəhddən  sonra  heasb  bloklanır
##  HOME  PAGE
- ### Home  page düzgün  açılır və  page  title  düzgün   göstərilir
- ### Baş menyu elementləri  görünür menyu  uzərində hover kliklər düzgün  işləyir
- ### Hər  bir menyu  düzgün  səhifəyə  yönləndirir
- ### Reklam  bannerləri  və  əməliyyatların  icra  butonları  düzgün işləyir
- ### Bannerlər  kilkləndikdə  düzgün  səhifəyə  keçid olur
- ### Kart  hesabları  ana səhifədə  görünür
- ### ƏDV , Keşbek, Bonus  əməliyyatları  ana səhifədə   görünür
- ### Butun keşbek, ƏDV balansları  düzgün  göstərilir
- ### ƏDV  və Keşbek  məbləğləri  düzgün  hesablanır
 ## İstifadəçi   Profili
- ### Profil  məlumatları ( ad,  soyad,email və  telefon  nömrəsi )  düzgün  göstərilir 
- ### Tətbiqə giriş  üçün  barmaq  izi  və Passcode seçimi  aktivdir
- ### Profil  dəyişdirildikdən  sonra yeniliklər  yadda   qalır
- ### Logout   fünksiyası  düzgün  işləyir
 ## Hesablar   və  Balans
- ### İstifadəçiyə   məxsus   bütün  hesablar  gösterilir
- ### Hər bir  hesab  üçün Cari  balans  düzgün   göstərilir
- ### " Gizlədilmiş  məhsulları   göstər "   fünksiyası  düzgün  işləyir
- ### Hesab  məlumatları   düzgün açılır
- ### Valyuta    düzgün  göstərilir ( AZN / USD /EUR )
##  Pul  Köçürmələri
  - ### Mənim  kart  hesablarım  arasında  kğçürmə  mümkündür
  - ### İstənilən  bank  kartına  köçürmə  mümkündür
  - ### Dosta  köçürmə  və  dostlardan  pul  sorğusu  əməliyyatları  işləyir
  - ### Məbləğ   sıfır  olduqda köçürməyə  icazə  verilmir
  -  ### Mənfi və  simvol daxil edilmiş   məbləğ  qəbul  edilmir və " Məbləğ  düzgün  deyil" xəbərdarlıq  mesajı gəlir
  -  ### Cari  balansdan  kifayət   yüksək   məbləğ  daxil  edildikdə "Balansınız  kifayət  deyil" xəbərdarlıq mesajı  gəlir
  -  ### Köçürmə  məbləği  minimum limitdən aşağı olduqda "Minimüm  köçürme məbləği X AZN-dır" və  maksimum limitdən yüxarı  olduqda"maksimüm köçürmə məbləği Y AZN-dir" xəbərdarlıq  mesajı  gəlir 
  -  ### Pul köçürülməsidə  kart nömrəsinin skan edilməsi zamanı  kart  nömrəsi düzgün şəkildə daxil olur
  -  ### Pul  köçürməsi  zamanı  təstiq  mesajı  (OTP / SMS )  gəlir
  -  ### OTP düzgün daxil  ediləndə əməliyyat uğurlu  olur
  -  ### Səhv  OTP  daxil  edildikdə "Xahiş  olunur  düzgün  OTP daxil  edin" mesajı göstərilir
  -  ### OTP  müddəti bitdikdə - "OTP  vaxtı  bitdi ,yenidən göndərin " mesajı  göstərilir
  -  ### Köçürmə  uğurlu  olduqda  bildiriş  mesajı  gəlir
    
 ##   Əməliyyat  tarixçəsi testi
- ### Tarixçə  səhifəsi   açılır
- ### Əməliyyatlar  tarixə  və növə  görə  sıralanır
- ### Fitrləmə  tarix,  növ  və  məbləğə  görə  düzgün  işləyir
- ### Bütün  əməliyyat   detalları   tam  göstərilir  ( məbləğ , tarix , status , alıcı )
 ## UI / UX testing
 - ### Butun   düymələr  klik  olunur
 - ### UI  elementləri  ust-üstə  düşmür
 - ### Mətnlər  oxunaqlıdır
 - ### Xəta  mesajları  aydındır
 ## SECURİTY testing
 - ### HTTPS   protokolu  istifadə  olunur
 - ### URL   dəyişdirilərək   başqa  hesaba  giriş  mümükn  deyil
 -  ### Şəxsi  məlumatlar  açıq  görünmür
 - ### Kart  məlumatları  açıq olduqda  screenshots   mümkün  deyi
 - ### Login  sonrası  Back  düyməsi  ilə  geri  qayıtmaq  olmur
  ## Performance Testing
 - ### Səhifələr  3 saniyədən  gec  yüklənmir
 - ### Yüklənmə  zamanı  sistem  donmur
 - ### Pul  köçürməsi  zamanı  gecikmə  yoxdur
## Compatiblity  testing
 - ### Tətbiqin  bütün fünksiyaları  fərqli   cihazlarda- Desktop,tablet,mobilde düzgün  işləyir
 -  ### Fərqli  əməliyyat  sistemlərində - Windows , MacOS, Android, IOS  əməliyyat  sistemlərində  düzgün  işləyir
 - ###  Fərqli brauzerlərdə -  Chrome, Firefox, Edge ,Opera, Safaride stabil  işləyir

































    
    
