## Test Case 1
## Test Case ID:TC_001
## Title:Valid məlumatlarla Login fünksiyasının yoxlanışı
## Preconditions: İstifadəçi  sistemdə  qeydiyyatdan  keçib

|steps|   Action               |    Data              |    Expected Result                                   |    Actual Result     |
|-----|------------------------|----------------------|------------------------------------------------------|----------------------|
|1    |Kapital bank veb saytını aç|                   |Kapital bank veb saytı açılır                         |  Sayt açılır         |                      
|2    |Login səhifəsini aç     |                      |  Səhifə açılmalıdır                                  |Login səhifəsi açılır |
|3    | Email sahəsinə valid  email daxil et   | pervinferzi@gmail.com| Məlumat email sahəsində görünməlidir                 | Email düzgün xanada görünür|
|4    | Password sahəsinə valid password daxil et | H1234%miko           |  Password şifrə sahəsində görünməlidir               | Password düzgün xanada görünür 
|5    |Login düyməsinə click et|                      | Istifadəçi girişi uğurlu olmalı,profil səhifəsi açılımalıdır | Giriş uğurlu oldu və profil səhifəsi açıldı |



## Test case 2
## Test case ID: TC_002
## Title: Invalid məlumatlarla Login funksiyasının yoxlanışı
## Precondition:Qeydiyyatdan keçmiş istifadəçi mövcüddür
| Steps| Action                                  |    Data                 |   Expected Result                |  Actual Result         |
|------|-----------------------------------------|-------------------------|----------------------------------|------------------------|
|1     |  Login səfifəsini aç                    |                         | Login səhifəsi açılmalıdır           | Login səhifəsi açıldı |
|2     | Email sahəsinə  invalid email  daxil et |  perH1234@gmail.com     |Məlumat email sahəsində görünməlidir   |  Email düzgün xanada görünür |
|3     | Password sahəsinə invalid şifrə daxil et|  M1237#qa               |Şifrə password xanasında görünməlidir  |Password düzgün xanada görünür  |
|4     |Login düyməsinə click et                 |                         |İstifadəçi sistemə daxil olmamalıdır   |"Daxil etdiyiniz Email və ya şifrə yanlışdır" xəta mesajı gəlir|

## TEST CASE 3
## Test Case ID : TC_003
## Title : Boş email və şifrə ilə Login funksiyasının yoxlanışı
## Precendition : Login səhifəsi açıqdır
|Steps|   Action                   | Data  |   Expected Result                              |  Actual   Result                           |
|-----|----------------------------|-------|------------------------------------------------|--------------------------------------------|
|1    |Email sahəsini boş saxla    |       |Email xanasında heçnə yazılmamalıdır            |Email sahəsi boşdur                         |
|2    |Password  sahəsini boş saxla|       |Şifrə sahəsi boş olmalıdır                      |Password sahəsi boşdur                      |
|3    |"Login " düyməsini clicklə  |       |Xəta mesajı çıxmalıdır və login baş verməməlidir| "Please fill out this field" mesajı göndərilir  |


## Test Case 4
## Test Case ID : TC_004
## Title:Uğurlu  pul  köçurmə  əməliyyatı
## Precondition : Istifadəçi login  olmuşdur və hesabda kifayət qədər  balans var

| Steps| Action                        |  Data             | expected Result                                                   | Actual result                    
|------|--------------------------------|--------------------|-------------------------------------------------------------------  |-----------------------------|
|1     |Kapital Bank veb tətbiqini aç|                    | Veb tətbiqin home page görünməlidir                                    | Dashboard açıldı                   
|2     |"Pul köçürmə " bölməsinə keç |                    | Pul köçürmə səhifəsi açılmalıdır                                       |Pul köçürmə səhifəsi açıldı                    
|3     | Kart nömrəsini daxil et     |1234 5678 9768 1090 |Kart nömrəsi xanada görunməlidir                                        |Kart nömrəsi xanada görünür         
|4     | Köçürmə məbləği daxil et    | 50 AZN             | Daxil edilən məbləğ xanada görünməlidir                                |Köçürmə məbləği xanada görünür|
|5     | "Köçür" düyməsinə click et  |                    |əməliyyatın icrası başlamalıdır                                         | Prosses başlayır            |
|6     |Əməliyyatı təstiqlə          |                    | Pul uğurla köçürülür "Əməliyyat uğurla tamamlandı" mesajı göstərilməlidir|Köçürmə uğurla tamamlandı və təstiq mesajı gəldi     
                                                                           
## TEST CASE 5
## Test Case ID: TC_005
## Title : Balansdan artıq məbləğin köçürülməsi
## Precondition :İstifadəçi login olmuşdur və  hesab balansı köçürülən məbləğdən azdır(Balans 500 AZN)

|Steps| Action                          |Data               | Expected Result                  | Actual Result                                 |
|-----|---------------------------------|-------------------|-----------------------------------|-----------------------------------------------|
|1    |Kapital bank tətbiqini aç        |                   | Tətbiq açılmalıdır                |Tətbiq açılır və home page görünür             |
|2    |Pul köçürmə səhifəsinə keç       |                   | Köçürmə səhifəsinə daxil olmalıdır| Pul köçürmə səhifəsi açılır                   |
|3    |Kart nömrəsini daxil et          |1997 2026 2021 1992| Nömrə uyğün xanada görünməlidir   |Kart nömrəsi düzgün xanada görünür             |
|4    |cari balansdan yuksək məbləğ daxil et |800 AZN            |Məbləğ uyğun xanada görünməlidir   |Məbləğ düzgün xanada görünür                   |
|5    |Köçür düyməsinə click et         |                   |Xəbərdarlıq mesajı gəlməlidir      | Balans kifayət deyil xəbərdarlıq mesajı gəlir |



                      
## TEST CASE 6
## Test Case ID: TC_006
## Title : Mənfi və sıfır məbləğ ilə pul transferi
## Precondition :İstifadəçi veb tətbiqdə login olmuşdur 

|Steps| Action                            |Data               | Expected Result                   | Actual Result                                 |
|-----|-----------------------------------|-------------------|-----------------------------------|-----------------------------------------------|
|1    |Kapital bank tətbiqini aç          |                   | Tətbiq açılmalıdır                |Tətbiq açılır və home page görünür             |
|2    |Pul köçürmə səhifəsinə keç         |                   | Köçürmə səhifəsinə daxil olmalıdır| Pul köçürmə səhifəsi açılır                   |
|3    |Kart nömrəsini daxil et            |1997 2026 2021 1992| Nömrə uyğün xanada görünməlidir   |Kart nömrəsi düzgün xanada görünür             |
|4    |Məbləğ sahəsinə köçürmə məbləği yaz|     0 AZN         |Xəbərdarlıq mesajı çıxmalıdır      |"Minimal dəyər 1.00 AZN olmalıdır" mesajı çıxır|
|5    |Məbləğ sahəsinə mənfi ədəd yaz     |  -50 AZN          |Mənfi dəyər qəbul olunmamalıdır    |Sistem mənfi dəyəri qəbul etmir                |


          
## TEST CASE 7
## Test Case ID: TC_007
## Title : Yanlış kart  nömrəsi ilə transfer
## Precondition :İstifadəçi veb tətbiqdə login olmuşdur 

|Steps| Action                           |Data                | Expected Result                   | Actual result                                 |
|-----|-----------------------------------|-------------------|-----------------------------------|-----------------------------------------------|
|1    |Kapital bank tətbiqini aç          |                   | Tətbiq açılmalıdır                |Tətbiq açılır və home page görünür             |
|2    |Pul köçürmə səhifəsinə keç         |                   | Köçürmə səhifəsinə daxil olmalıdır| Pul köçürmə səhifəsi açılır                   |
|3    |Kart nömrəsini daxil et            |1997 2026 2021 1992| Nömrə uyğün xanada görünməlidir   |Kart nömrəsi düzgün xanada görünür             |
|4    |Məbləğ sahəsinə köçürmə məbləği yaz|     100 AZN       |Xəbərdarlıq mesajı çıxmalıdır      |"Minimal dəyər 1.00 AZN olmalıdır" mesajı çıxır|
|5    |"Göndər" düyməsinə click et        |                   |Xəbərdarlıq mesajı çıxmalıdır      |"Kart nömrəsi yanlışdır" mesajı çıxır          |   




## TEST CASE 8
## Test Case ID: TC_008
## Title : Düzgün OTP kodu ilə təstiq
## Precondition :İstifadəçi veb tətbiqdə login olmuşdur.Transfer əməliyyatı başladılıb 

|Steps| Action                           |Data                | Expected Result                   | Actual result                                 |
|-----|-----------------------------------|-------------------|-----------------------------------|-----------------------------------------------|
|1    |Kapital bank tətbiqini aç          |                   | Tətbiq açılmalıdır                |Tətbiq açılır və home page görünür             |
|2    |Pul köçürmə səhifəsinə keç         |                   | Köçürmə səhifəsinə daxil olmalıdır| Pul köçürmə səhifəsi açılır                   |
|3    |Kart nömrəsini daxil et            |1997 2026 2021 1992| Nömrə uyğün xanada görünməlidir   |Kart nömrəsi düzgün xanada görünür             |
|4    |Məbləğ sahəsinə köçürmə məbləği yaz|     100 AZN       |Məbləğ düzgün xanada görünməlidir  |Daxil edilmiş məbləğ düzgündür                 |
|5    |"Göndər" düyməsinə click et        |                   |Transfer əməliyyatı  başlamalıdır  |Köçürmə icra olunmağa başlayəır                | 
|6    |SMS bölməsinə gələn OTP kodu daxil et| XXXXXX          |Kod düzgün xanada görünməlidir     |Kod uyğun xanadadır                            |
|7    |Təstiqlə düyməsini kliklə            |                 | Əməliyyat icra olunmalıdır        | Pul transferi uğurlu olur və təstiq  mesajı  göndərilir |




## TEST CASE 9
## Test Case ID: TC_009
## Title : Eyni  OTP-nin  təkrar istifadəsi
## Precondition :İstifadəçi veb tətbiqdə login olmuşdur .Transfer əməliyyatı uğurla OTP ilə tamamlanmışdır

|Steps| Action                           |Data                | Expected Result                   | Actual result                                 |
|-----|-----------------------------------|-------------------|-----------------------------------|-----------------------------------------------|
|1    |Kapital bank tətbiqini aç          |                   | Tətbiq açılmalıdır                |Tətbiq açılır və home page görünür             |
|2    |Pul köçürmə səhifəsinə keç         |                   | Köçürmə səhifəsinə daxil olmalıdır| Pul köçürmə səhifəsi açılır                   |
|3    |Transfer əməliyyatını OTP ilə uğurla tamala|  XXXXXX  | Əməliyyat uğurla bitməlidir       |Transfer uğurlu olur və təstiq mesajə göndərilir|
|4    |Eyni OTP kodu ilə yeni transfer başlat|                |Əməliyyat başlamalıdır             |Təkrar transfer əməliyyatı başlayır             |
|5    |OTP sahəsinə əvvəlki kodu daxil et | XXXXXX            |Kod uyğun xanada görünməlidir      | Kod düzgün xanada görünür                      |
|6    |"Təstiq et" duyməsinə kliklə         |                   |Sistem OTP ni qəbul etməməlidir.Xəbərdarlıq mesajı çıxmalıdır|OTP qəbul olunmur."OTP artıq istifadə olunub" mesajı çıxır.Əməliyyat icra olunmur



## TEST CASE 10
## Test Case ID: TC_10
## Title : Yanlış  OTP daxil edilməsi
## Precondition :İstifadəçi veb tətbiqdə login olmuşdur .


|Steps| Action                           |Data                | Expected Result                   | Actual result                                 |
|-----|-----------------------------------|-------------------|-----------------------------------|-----------------------------------------------|
|1    |Kapital bank tətbiqini aç          |                   | Tətbiq açılmalıdır                |Tətbiq açılır və home page görünür             |
|2    |Pul köçürmə səhifəsinə keç         |                   | Köçürmə səhifəsinə daxil olmalıdır| Pul köçürmə səhifəsi açılır                   |
|3    |Kart nömrəsini daxil et            |1234 5678 9123 4582| Nömrə uyöun xanada görünməlidir   |Kart nömrəsi düzgün xanada görünür             |
|4    |Köçürmə məbləğini daxil et         |  500 AZN          |Məbləğ düzgün xanada görünməlidir  |Məbləğ uyğun xanada görünür                    |
|5    |OTP sahəsinə yanlış kodu daxil et  | XXXXXX            |Kod uyğun xanada görünməlidir      | Kod düzgün xanada görünür                      |
|6    |"Təstiq et" duyməsinə kliklə       |                   |Sistem OTP ni qəbul etməməlidir.Xəbərdarlıq mesajı çıxmalıdır|OTP qəbul olunmur.Əməliyyat icra olunmur



## TEST CASE 11
## Test Case ID: TC_11
## Title : SQL  injection yoxlanışı
## Precondition :İstifadəçi login  səhifəsi açıqdır.


|Steps| Action                           |Data                | Expected Result                   | Actual result                                 |
|-----|-----------------------------------|-------------------|-----------------------------------|-----------------------------------------------|
|1    |Kapital bank tətbiqini aç          |                   | Tətbiq açılmalıdır                |Tətbiq açılır və home page görünür             |
|2    |Username sahəsinə ' OR '1'='1 daxil et| '1'='1         | məlumat uyöun xanada olmalıdır    |yazdığımız username düzgün xanadadır           |
|3    |Password sahəsinə istənilən şifrə yaz |Mek2021%nem     | şifrə uyğun xanada görünməlidir   |şifrə düzgün xanada görünür             |
|4    |Login et düyməsinə clicklə         |                   |Login uğursuz olmalıdır            |Login uğursuz olur database istifadəçiyə göstərilmir.Məlumat bazası təhlukəsizdir









