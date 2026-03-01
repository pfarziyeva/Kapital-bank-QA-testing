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

|Steps| Action                            |Data               | Expected Result                   Actual Result                               |
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

