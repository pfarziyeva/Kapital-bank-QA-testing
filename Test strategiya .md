
## Projekt name
### Kapital Bank veb tətbiqi 
  ## Hazırlayan : Pərvin  Hümmətova
 ## MƏQSƏD
 - ### Kapital  Bank veb tətbiqinin istifadəçi tələblərinə uyğun işlədiyini yoxlamaq 
 - ### Kritik  bank  əməliyyatlarında xətaların qarşısını almaq
- ### istifadəçi məlumatlarının təhlukəsizliyini  təmin etməkdir.
 ## TEST SKOPE ( In Scope)
 - ### Istifadəçi giriş və çıxışı (LOGİN /LOGOUT )
 - ### Hesab balansının görüntülənməsi - Cari balansdakı məbləğin düzgün göstərilməsi
 - ### Pul köçürmələri
  ### - Kartddan karta  transfer ( Eyni  bank  daxilində  ödənişlər  və  muxtəlif  banklararası  ödənişlər  )
### - Hesabdan   hesaba  transfer  ( Fərdi  hesablar  arasında   )
### - Ödəniş  məbləği  yoxlaması  (Mənfi  və  sıfır  məbləğin  qəbul  edilməməsi)
 - ### Kartların idarə olunması (bloklama, limit dəyişmə)
 - ### Bildirişlər və əməliyyat tarixçəsi
 - ### Ödənişlər (kommunal, mobil ,internet ödənişlər)
## Out Of Scope
- ### Production -  da   real  pul əməliyyatları.  Real ödəniş  və köçürmələr test olunmur
- ### Backend optimizasiya və server performansı.  Testçi  serverin  sürətini  və optimizasiyasını  yoxlamır
  ##  TEST  Approach
  - ### Test  staging  mühitdə  manual şəkildə   həyata  keçiriləcək. Fünksional  və  Non  functional  test   növlərindənn istifadə  etməklə  saytın bütün fünksiyalarının  düzgün  işləməsini  və    eyni  zamanda  istifadəçi  tələblərinə  uyğunluğunu təmin   etmək  məqsədi ilə bank  veb  tətbiqi  test  olunacaq. 
  -
 ## TEST  Types :
   ## Functional   Testing -  Saytın  bütün  əsas   fünksiyalarının  düzgün  işləməsini  təmin etmək  üçün  həyata  keçirilir.
  - ### Smoke test - Saytın vacib bir  fünksiyasına  fokuslanaraq  sürətli yoxlanış  üçün  həyata  keçirilir.
  - ### Regression test - saytda müəyyən bir fünksional  dəyişiklikdən  sonra  əvvəlki fünksiyaların  düzgün işləməsini yoxlamaq üçün aparılır.
  - ### Unit Test -  Proqramın  hər bir  kiçik  vahidinin  fünksionallığını  yoxlayır
  -  ### Sanity Test -  Sistemdə  kiçik  dəyişiklikdən  sonra  məsələn  bug  fix  edildikdən  sonra  əsas  fünksiyanın  hələdə  işlədiyini  yoxlamaq  üçündür.
 ## Non Fünctional  Testing :
  - ### UI / UX  test - Saydın  ümümi  dizaynı  və  istifadəçinin  saytdan  rahat  şəkildəə istifadə  etməsini  təmin   etmək   məqsədi  daşıyır.
  - ### Security test -   İstifadəçi   məlumatlarının  təhlukəsizliyini  təmin  etmək  məqsədi  ilə  aparılır.
  - ### Performance  Test - Saytın   yuklənmələrə  qarşı  dözümluluyünu  test edir
  - ### Usibility  test - İstifadəçi  saytda  müəyyən  əməliyyatları  icra   edərkənn çətinlik  çəkməməsi  üçün həyata keçirilir.Məsələn  buttonları  rahat  tapa
    bilsin , forma dolduran  zaman   mərhələlər  aydın  və   qısa olsun və.s
    ## Test  Data  :
    - ### Pozitiv  test data  -  doğru  login məlumatları ,   kifayət  qədər  balans ,   düzgün  kart/ IBAN
    - ### Negative  test   data  - Səhv  parol ,   kifayət  qədər  balans  yoxdur   və  yanlış  IBAN
    - ###  Sərhəd  Test  data -  minimum / maksimum  məbləğ  və  günlük  limitin  tam  həddi
    ## Entry  Criteria
    - ### Requirements  təstiqlənib
    - ### Test plan   və  Test strategiya  hazırdır
    - ### Staging yəni  test  mühiti  qurulub  və  işləkdir
    -  ### Test   data  mövcüddür
 ## TEST ENVİRONMENT
 - ### Environment : Staging 
 - ### OS : Windows 11 ,Android/Ios 
 - ### Brauzer : GOOGLE Chrome ,Firefox  ,  Edge
 - ### Cihazlar : Tablet , Mobil
 ## Test Tools:
  - ### Jira /  Bugzilla  -  Bug  tracking
  -  ### Postman  - API testleri
  -  ### TestRail / Qase -  Test  case yazlması  üçün
  -  ### JMeter - Performance test aleti
 ## ROLLAR
 - ### Project Manager
 - ### Developer
 - ### QA Engineer
 ##  TEST  SƏNƏDLƏRİ
### - Test Case - Hər hansı  bir  fünksiyanın  adddım -addım yoxlanışını  təmin edir
### - Checklist -  Ümümi   yoxlanış  siyahısıdır
### - Bug report- Tapılmış  bugın sənədləşdirilməsi
### - Test plan sənədi
### -  Test summary report - Test  sonunda  
 ## RISKLƏR
## 1) LOGIN funksiyası ilə bağlı risk
  ### - Istifadəçi düzgün məlumat daxil etsə də sistemə daxil ola bilməməsi
 ### - Yanlış şifrə bir neçə dəfə daxil edildikdə hesabın bloklanmaması
##  2) Pul köçürmələrində səhvlər
  ### - Pul köçürmələrinin yarımçıq və ya səhv tamamlanması
  ### - Pul hesabdan  çıxır amma qarşı tərəfə çatmır
  ### - Yanlış məbləğin  köçurulməsi 
  ### - Ikiqat pul  transferi
  ### -Yanlış  IBAN - a   Pul  köçürülməsi  və  pulun  geri  qaytarılmaması
## 3) Balansın səhv göstərilməsi
 ### - Heasb balansının real məbləğə uyğun olmaması
## 4) Ödənişlərin təstiqlənməməsi
 ### - Kommunal mobil və ya internet ödənişləri tamamlanmaya bilər. 
### - Balansdan vəsait çıxır amma ödəniş təstiqlənmir.
## 5) Tətbiqin donması və ya bağlanması
- ### Əməliyyat zamanı tətbiqin dayanması cari əməliyyatların yarımçıq qalması ilə nəticələnir
## 6 ) Təhlukəsizlik boşluqları
- ### Məsələn səhv şifrəni çox yazanda hesab bloklanmaması  Hacker hucumlarına şərait yaradır
  ##  Exit Criteria
  - ### Critical  və  high  severity  bug-lar  bağlanıb   və retest  olunub
  -  ### Test  case-lərin  ən az   95 % -i   icra  olunub
  -  ###  Planlaşdırılan    testlər    tamamlanıb və  test   nəticələri  sənədləşdirilib
  -  ### Test  Summary  Report  hazırlanıb




 
