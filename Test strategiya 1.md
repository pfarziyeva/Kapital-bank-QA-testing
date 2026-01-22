##  Test Strategiya
## Projekt name
### Kapital Bank veb tətbiqi 
 ## MƏQSƏD
 -  Kapital  Bank veb tətbiqinin istifadəçi tələblərinə uyğun işlədiyini yoxlamaq 
 - Kritik  bank  əməliyyatlarında xətaların qarşısını almaq
- istifadəçi məlumatlarının təhlukəsizliyini  təmin etməkdir.
 ## TEST SKOPE ( In Scope)
 - Istifadəçi giriş və çıxışı (LOGİN /LOGOUT )
 - Hesab balansının görüntülənməsi - Cari balansdakı məbləğin düzgün göstərilməsi
 - Pul köçürmələri (Öz hesabları arasında və digər şəxslərə pul köçürmə)
 - Kartların idarə olunması (bloklama, limit dəyişmə)
 - Bildirişlər və əməliyyat tarixçəsi
 - Ödənişlər (kommunal mobil internet ödənişlər)
## Out Of Scope
- Production -  da   real  pul əməliyyatları.  Real ödəniş  və köçürmələr test olunmur
- Backend optimizasiya və server performansı.  Testçi  serverin  sürətini  və optimizasiyasını  yoxlamır
  ##  TEST  Approach
  -
 ## TEST  NÖVLƏRİ
  - Funksional test -  Saytın  bütün  əsas   fünksiyalarının  düzgün  işləməsini  təmin etmək  üçün  həyata  keçirilir.
  - Smoke test - Saytın vacib bir  fünksiyasına  fokuslanaraq  sürətli yoxlanış  üçün  həyata  keçirilir.
  - Regression test - saytda müəyyən bir fünksional  dəyişiklikdən  sonra  əvvəlki fünksiyaların  düzgün işləməsini yoxlamaq üçün aparılır.
  - UI / UX  test - Saydın  ümümi  dizaynı  və  istifadəçinin  saytdan  rahat  şəkildəə istifadə  etməsini  təmin   etmək   məqsədi  daşıyır.
  - Security test -   İstifadəçi   məlumatlarının  təhlukəsizliyini  təmin  etmək  məqsədi  ilə  aparılır.
  -  Performance  Test - Saytın   yuklənmələrə  qarşı  dözümluluyünu  test edir
  -  Usibility  test - İstifadəçi  saytda  müəyyən  əməliyyatları  icra   edərkənn çətinlik  çəkməməsi  üçün həyata keçirilir.Məsələn  buttonları  rahat  tapa  bilsin , forma dolduran  zaman   mərhələlər  aydın  və   qısa olsun və.s
 ## TEST ENVİRONMENT
 - OS : Windows 11 ,Android/Ios 
 - Brauzer: GOOGLE Chrome
 ## ROLLAR
 - Project Manager
 - Developer
 - QA Engineer
 ##  TEST  SƏNƏDLƏRİ
 - Test Case - Hər hansı  bir  fünksiyanın  adddım -addım yoxlanışını  təmin edir
 -  Bug report- Tapılmış  bugın sənədləşdirilməsi
 -  Test summary report - Test  sonunda  
 ## RISKLƏR
## 1) LOGIN funksiyası ilə bağlı risk
-  Istifadəçi düzgün məlumat daxil etsə də sistemə daxil ola bilməməsi
. Yanlış şifrə bir neçə dəfə daxil edildikdə hesabın bloklanmaması
##  2) Pul köçürmələrində səhvlər
 - Pul köçürmələrinin yarımçıq və ya səhv tamamlanması
 - Pul hesabdan  çıxır amma qarşı tərəfə çatmır
## 3) Balansın səhv göstərilməsi
-   Heasb balansının real məbləğə uyğun olmaması
## 4) Ödənişlərin təstiqlənməməsi
-   Kommunal mobil və ya internet ödənişləri tamamlanmaya bilər. 
- Balansdan vəsait çıxır amma ödəniş təstiqlənmir.
## 5) Tətbiqin donması və ya bağlanması
-  Əməliyyat zamanı tətbiqin dayanması cari əməliyyatların yarımçıq qalması ilə nəticələnir
## 6 ) Təhlukəsizlik boşluqları
-  Məsələn səhv şifrəni çox yazanda hesab bloklanmaması  Hacker hucumlarına şərait yaradır




 
