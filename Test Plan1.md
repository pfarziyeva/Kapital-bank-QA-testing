## Project name :   Kapital Bank veb tətbiqi
## Hazırlayan:  Pərvin Hümmətova
## Test Növü: MANUAL TESTİNG
## Testin başlama və bitmə tarixi: 18/01/2026 - 21/01/2026
# Məqsəd :
## Tətbiqin əsas fünksiyalarının  düzgün işlədiyini yoxlamaq, səhvləri  erkən aşkar etmək və istifadəçi təcrübəsinin sabitliyini təmin etməkdir.
# Test Skope  ( İN Scope)
  - ## İstifadəçi qeydiyyatı və login
  - Hesab balansının yoxlanması
  - Pul köçürmələri  ( Öz hesablarım və istənilən bank kartına köçürmə )
  - Kart idarəetməsi (bloklama, limit dəyişimi)
  - Ödəniş əməliyyatları ( Kommunal, mobil , internet )
  - Əməliyyat tarixçəsi və bildirişlərin yoxlanması
  - Dil seçimi ( AZ /EN/ RU )
  - UI/UX - saytın ümümi dizaynı və istifadəçi üçün rahat istifadəni   təmin etmək
  - Logout
  # Out of Scope
  - Real maliyyə əməliyyatları
  - Core banking  sistemi əməliyyatları( Backend serverdə maliyyə  əməliyyatları)
  - Üçüncü tərəf daxili sistemləri ( məsələn bankın daxili audit sistemi)
 # Entry Criteria
- Testin başlaya bilməsi üçün :
- Test ediləcək tətbiq staging mühitində hazır olmalıdır
- Bütün əsas fünksiyalar tətbiqdə mövcüd olmalıdır
- Test data hazırlanmalıdır ( hesablar istifadəçi məlumatları)
- Test mühiti (browser, OS alətlər ) işlək vəziyyətdə olmalıdır
- Test sənədləri hazır olmalıdır
  # Test Data
  - Düzgün və yanlış Login məlumatları
  - Test istifadəçi hesabları
  - Saxta kart nömrələri
  - Minimum, maksimum və yanlış köçürmə məbləğləri
  # Test Environments :
  - OS : Mobil( Android / İOS ), Windows 11,macOS
  - Browser: GOOGLE CHROME ,Firefox
  - Network : Internet  bağlantısı
  # Test Approach
 - Testlər manual şəkildə aparılacaq
 - Hər test fünksiyası üçün test case hazırlanacaq
 - Test nəticəsində bug varsa bug report hazırlanacaq
- Kritik xətalar dərhal komanda ilə paylaşılacaq
 # Test növləri
## Fünctional  Testing : 
- SMOKE test ( əsas funksiyalar sürətli test olunur )
- Regression test (Əvvəlki testlərdə işləyən fünksiyalar yenidən yoxlanılacaq)
- Acceptance  Testing ( UAT) - Sitemin  biznes  tələblərinə  uyğun  olub olmadığını  yoxlamaq  məqsədi  iləı  aparılır
  ## Non Fwnction Testing :
- Uİ/UX Test - İstifadəçinin saytda gördüyü elementlərin düzgün olması və istifadə rahatlığının təmin edilməsi
- Security test-Tətbiqdə istifadəçi  məlumatlarının və əməliyyatlarının  qorunması üçün aparılır
- Compatiblity test - Fərqli cihaz , muhit  və  platformada tətbiqin düzgün işləməsini təmin etmək üçün aparılır
- Performance test - Tətbiqin yüklənməsi zamanı işləmə qabiliyyətini yoxlamaq üçün istifadə olunur
# TOOLS
- Jira / Zephyr (Bug reporting və test case idarəsi üçün )
- Test manegement: TestRail / Qase
# Test Deliverables: 
- Test strategiya sənədi
- Test  plan ssənədi
- Test caselər
- Bug report
- Test summary report
  
  # ROLLAR
  - QA Enginner
  - Developer
  - Product Owner
  - Projekt Manager
# RİSKLƏR
## Hight Severity Risklər:
-  Ödəniş əməliyyatının düzgün işləməməsi:
  1) Ödəniş uğurlu görünür amma realda icra olunmur
  2) Eyni ödəniş bir neçə dəfə təkrarlanır
  3) Balans kifayət etmədiyi halda ödəniş icra olunur
-  Pul köçürməsi zamanı risklər:
  1) Muştəri IBAN ı səhv yazır və pul başqa hesaba gedir. Bu zaman pul geri qaytarılmaya bilər
  2) Pul iki dəfə köçürülə bilər
  3) Pul çıxır amma qarşı tərəfə çatmır   
- Avtorizasiya və acces control zəifliyi ( istifadəçi başqasının hesabına daxil ola bilər)
  
   İstifadəçinin icazəsi olmayan hesablar  üzərində əməliyyat apara bilməsi
  
   URI və API parametrlərinin dəyişdirilməsi ilə icazəsiz məlumat əldə edilməsi
  
-  Şifrə  bərpası və autentifikasiya prosesində boşluqlar (Müştəri hesabına icazəsiz giriş, məlumatların sızması)
  
## Medium severity risklər:
- Hesab çıxarışının yavaş yüklənməsi
- müəyyən brauzerlərdə səhifə formatının pozulması
## Low severity risklər:
- UI elementlərinin kiçik dizayn problemi
- Yazıların doğru olmaması
#  Exit Criteria :
## Test prosesinin tamamlanması üçün :
- Bütün  critical və high severity buglar fix olunub
- Test  caselərin  95% -i uğurlu keçib
- Bütün kritik fünksiyalar işləkdir
-  Test nəticələri sənədləşdirilib
-   Test  Summary  Report hazırlanıb
  #  NƏTİCƏ
  ## Bu  test  plan  bank  veb  tətbiqinin keyfiyyət , təhlukəsizlik  və  istifadəçi   tələblərinəə tam  uyğun  şəkildə  qurulmasını  təmin etmək  məqsədi  ilə  hazırlanmışdır .  Test  prosesində   əsas  yol  xəritəsi  rolunu  oynayan  vacib  dakumentasyadır.
  


 
