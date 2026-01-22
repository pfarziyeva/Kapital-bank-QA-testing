# Project :  Kapital Bank veb tətbiqi
# Hazırlayan: Pərvin Hümmətova
# Testin başlama və bitmə tarixi:
## 18/01/2026 - 21/01/2026
# Məqsəd : Tətbiqin əsas fünksiyalarının  düzgün işlədiyini yoxlamaq, səhvləri  erkən aşkar etmək və istifadəçi təcrübəsinin sabitliyini təmin etməkdir.
# Test Skope  ( İN Scope)
  ## 1) İstifadəçi qeydiyyatı və login
  ## 2) Hesab balansının yoxlanması
  ## 3) Pul köçürmələri  ( Öz hesablarım və istənilən bank kartına köçürmə )
  ## 4) Kart idarəetməsi (bloklama, limit dəyişimi)
  ## 5) Ödəniş əməliyyatları ( Kommunal, mobil , internet )
  ## 6) Əməliyyat tarixçəsi və bildirişlərin yoxlanması
  ## 7) Dil seçimi ( AZ /EN/ RU )
  ## 8) Logout
  # Out of Scope
  ## Real maliyyə əməliyyatları
 ## core banking  sistemi əməliyyatları( Backend serverdə maliyyə  əməliyyatları)
 ## Üçüncü tərəf daxili sistemləri ( məsələn bankın daxili audit sistemi)
 # Entry Criteria
## Testin başlaya bilməsi üçün :
## Test ediləcək tətbiq staging mühitində hazır olmalıdır
## Bütün əsas fünksiyalar tətbiqdə mövcüd olmalıdır
## Test data hazırlanmalıdır ( hesablar istifadəçi məlumatları)
## Test mühiti (browser, OS alətlər ) işlək vəziyyətdə olmalıdır
## Test sənədləri hazır olmalıdır
  # Test muhiti
  ## OS : Mobil( Android / İOS ), Windows 11,macOS
  ## Browser: GOOGLE CHROME ,Firefox
  # Test Approach
  ## 1) Testlər manual şəkildə aparılacaq
 ## 2) Hər test fünksiyası üçün test case hazırlanacaq
  ## 3) Test nəticəsində bug varsa bug report hazırlanacaq
 ## 4) Kritik xətalar dərhal komanda ilə paylaşılacaq
 # Test növləri
## 1) SMOKE test ( əsas funksiyalar sürətli test olunur )
## 2) Fünksional test ( Bütün əsas əməliyyatlar test ediləcək)
## 3) Regression test (Əvvəlki testlərdə işləyən fünksiyalar yenidən yoxlanılacaq)
## 4) Exploratory test
## 5) Uİ/UX Test 
## 6) Security test
## 7) Compatiblity test
## 8) Performance test
# Alətlər 
## Jira /Zephyr (Bug reporting və test case idarəsi üçün )
## Test manegement: TestRail/Qase
# Test sənədləri
## Test caselər
## Bug report
## Test summary report
## Test strategiya sənədi
# RİSKLƏR
## Hight Severity Risklər:
### İstifadəçi məlumatlarının sızması
### Ödəniş əməliyyatının düzgün işdəməməsi yəni hesabdan artıq məbləğin çıxılması
### Avtorizasiya və acces control zəifliyi ( istifadəçi başqasının hesabına daxil ola bilər)
###  Şifrə  bərpası və autentifikasiya prosesində boşluqlar (Müştəri hesabına icazəsiz giriş, məlumatların sızması)
### əməliyyat prossesində kritik səhvlər (fund transfer) - Transfer səhv hesaba göndərilir və geri qaytarılmır
## Medium severity risklər:
### Hesab çıxarışının yavaş yüklənməsi
### müəyyən brauzerlərdə səhifə formatının pozulması
## Low severity risklər:
### UI elementlərinin kiçik dizayn problemi
### Yazıların doğru olmaması
#  Exit Criteria
## Bütün high severity buglar həll olunub
## Test  caselərin  95% -i uğurlu keçib
## Bütün kritik fünksiyalar işləkdir
## Test nəticələri sənədləşdirilib


 
