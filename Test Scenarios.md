# Kapital Bank web Application Test Scenarios
## Procekt : Kapital Bank web application
## Module :
- ## Authentication
- ## Accounts & Dashboard
- ## Funds Transfer
- ## Cards
- ## Payments
- ## Security & Session Managment
- ## UI/UX & Usability

 ## 1) Authentication module

## TS-01 -Verify successful login with valid registered user credentials
- ### Risk Level : Crirical
- ### Preconditions  :  İstifadəçi sistemdə qeydiyyatdan keçmişdir
- ### Test Scenario :  Düzgün email və şifrə daxil edərək sistemə giriş və Dashboard səhifəsinə  yönləndirmə mümkün olmalıdır.
  
  

## TS-02 - Verify system behavior for login attempt with invalid password
- ### Risk Level :  High
- ### Preconditions  :  İstifadəçi emaili sistemdə mövcüddür
- ### Test Scenario : İstifadəçi yanlış şifrə daxil etdikdə login cəhdi uğursuz olmalı və Password yanlışdır xəta mesajı göstərilir.

  

## TS -03 - Validate mandatory  field checks during login process
- ### Risk Level  :  Medium
- ### Preconditions :  Login  səhifəsi  əlçatandır
- ### Test Scenario  :  Email  və  şifrə  sahəsi  boş buraxılaraq login cəhdi uğursuz olmalı və muvafiq validasiya mesajları göstərilir və sessiya yaradılmır.

  

## TS -04 - Verify security control after  multiple  consecutive  failed  login attempts 
- ### Risk Level  :  High
- ### Preconditions :  İstifadəçi  hesabı aktivdir
- ### Test Scenario  :  5  ardıcıl uğursuz  login  cəhdindən sonra hesab  müvəqqəti bloklanır və istifadəçi xəbərdar edilir.



##  2) Accounts &  Dashboard  Module

## TS -05 - verify  correct display of account balance  after  successful authentication
- ### Risk Level :   Critical
- ### Preconditions : Aktiv  hesab  və login olmuş  istifadəçi   mövcuddur
- ### Test Scenario : Dashboard  səhifəsində  balans backend məlumatları  ilə uyğun  göstərilir.

  

## TS -06 - Verify automatic real-time balance update after financial transaction
- ### Risk Level :  High
- ### Preconditions :  Aktiv  hesab  və login olmuş  istifadəçi   mövcuddur
- ### Test Scenario : Transfer və ya ödəniş  etdikdən sonra balans avtomatik yenilənir  və düzgün  göstərilir

  

## TS -07 - Verify visibility and accuarcy  of transaction history records
- ### Risk Level :  Medium
- ### Preconditions : Aktiv  hesab  və login olmuş  istifadəçi   mövcuddur
- ### Test Scenario : Transaction history bölməsində əməliyyatlar düzgün  ardıcıllıqla və  məlumatlarla  göstərilir

  


## 3) Funds  Transfer  Module

## TS - 08  -  Verify successful internal  funds transfer between user accounts
- ### Risk  Level : Critical
- ### Preconditions  : Istifadəçi login olub və kifayət  qədər  balans mövcüddür
- ### Test  Scenario :  Transfer bölməsinə daxil ol, alıcı hesabı seç, məbləği  daxil  et  və  təstiqlə düyməsini  clicklədikdə transfer  uğurla  tamamlanır balans
yenilənir  və tranzaksiya tarixçəyə əlavə olunur.



## TS- 09 - Verify  system restriction when transfer amount exceeds available  balance
- ### Risk  Level:   High
- ### Preconditions :  Aktiv  hesab və login olunmuş  istifadəçi  mövcuddür
- ### Test Scenario :  Balansdan artıq məbləğ  daxil edilərək  transfer  cəhdi  zamanı  transfer bloklanır  və " İnsufficient balance " mesajı  göstərilir.
  

## TS- 10 - Validate transfer amount field for negative ,zero  and non-numeric inputs
- ### Risk  Level:  Medium
- ### Preconditions :  Aktiv  hesab və login olunmuş  istifadəçi  mövcuddür
- ### Test Scenario :  -10,0,"abc" və  digər uyğunsuz  dəyərlər  daxil  edildikdə bu dəyərlər rədd olunur ,uyğun  validasiya mesajları  göstərilir və  transfer  cəhdi uğursuz  olmalıdır.
  
  

## TS- 11 - Verify transfer attempt to  non -existing or invalid beneficiary account/card.
- ### Risk  Level:   High
- ### Preconditions :  Aktiv  hesab və login olunmuş  istifadəçi  mövcuddür
- ### Test Scenario :  Yanlış hesab /kart  nömrəsi  daxil edildikdə transfer icra  olunmur  və  uyğun xəta mesajı  göstərilməlidir.
  

## 4) Card Module

## TS-12- Verify display of user cards with  masked card number  format
- ### Risk Level :  High
- ### Precenditions :  Istifadəçinin  aktiv kartları mövcüddür
- ### Test Scenario :  Kart bölməsində kart nömrələri maskalanmış  formada göstərilir və  kart  detallarının mapping-i düzgün olmalıdır.

  


## TS-13- Verify correctness  of card details mapped to the authenticated user account
- ### Risk Level :  High
- ### Precenditions :  Aktiv  kartlar mövcüddür
- ### Test Scenario :  Kart detallarını   yoxlamaq və  hesabla uyğunluğunu  təstiqləmək
  
  
## 5) Payments Module

## TS-14- verify  successful execution of  utility bill payment with valid data
- ### Risk Level :  Critical
- ### Precenditions :  İstfadəçi login olub və kifayət qədər balans mövcüddür
- ### Test Scenario :  Payments bölməsində ödəniş  uğurla  tamamlanır, qəbz  göstərilir və  balans yenilənir

  


## TS-15- Verify system response for  payment attempt with invalid  subscriber information
- ### Risk Level : High
- ### Precenditions :  Aktiv  hesab  və login  olunmuş  istifadəçi  mövcüddür
- ### Test Scenario :  Yanlış abunə  kodu  daxil  etdikdə ödəniş  bloklanır və  xəta mesajı   göstərilməlidir
  

##  6) Security  & Session Management

## TS-16- Verify  automatic session termination after defined inactivity period 
- ### Risk Level :  Critical
- ### Precenditions :  İstifadəçi  login olmuşdur
- ### Test Scenario :  Sessiya  müddəti  bitdikdə sessiya bitir və  istifadəçi login  səhifəsinə  yönləndirməlidir
  


## TS-17-Verify prevention of unauthorized access to internal pages via direct  URL 
- ### Risk Level :  Critical
- ### Precenditions :  İstifadəçi login olmamışdır
- ### Test Scenario : Daxili  səhifənin URL ni birbaşa daxil  etdikdə sistem istifadəçini login  səhifəsinə yönləndirməlidir
  

## UI/UX  & Usability

### TS-18- Verify  responsive  layout across different screen resolutions
- ### Risk Level :  Medium
- ### Precenditions :  Web  tətbiq  açıqdır
- ### Test Scenario :  Desktop tablet və mobil  ölçülərdə layout uyğun görünməli , elementlər  kəsilməməli , istifadə  rahat   olmalıdır.
- 


##  TS-19- Verify proper navigation flow  through main menu links
- ### Risk Level :   Medium
- ### Precenditions :  Dashboard və ya home page  açıqdır
- ### Test Scenario :  Bütün  menü linkləri düzgün səhifələrə keçidi təmin  etməlidir.

