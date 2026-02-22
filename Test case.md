## Test Case 1
## Test Case ID:TC_001
## Title:Valid məlumatlarla Login fünksiyasının yoxlanışı
## Preconditions: İstifadəçi  sistemdə  qeydiyyatdan  keçib

|steps|   Action               |    Data              |    Expected Result                                   |    Actual REsult     |
|-----|------------------------|----------------------|------------------------------------------------------|----------------------|
|1    |Kapital bank veb Saytını aç|                   |Kapital bank veb saytı açılır                         |  Sayt açılır         |                      
|2    |Login səhifəsini aç     |                      |  Səhifə açılmalıdır                                  |Login səhifəsi açılır |
|3    | Email sahəsinə Valid  email daxil et   | pervinferzi@gmail.com| məlumat email sahəsində görünməlidir                 | Email düzgün xanada görünür|
|4    | Password sahəsinə Valid password daxil et | H1234%miko           |  password şifrə sahəsində görünməlidir               | password düzgün xanada görünür 
|5    |Login düyməsinə click et|                      | Istifadəçi girişi uğurlu olmalı.Profil səhifəsi açılımalıdır | Giriş uğurlu oldu və profil səhifəsi açıldı |



## Test case 2
## Test case ID: TC_002
## Title: Invalid məlumatlarla Login funksiyasının yoxlanışı
## Precondition:Qeydiyyatdan keçmiş istifadəçi mövcüddür
| Steps| ACTION                                  |    DATA                 |   EXPECTED  RESULT               |  ACTUAL  RESULT        |
|------|-----------------------------------------|-------------------------|----------------------------------|------------------------|
|1     |  Login səfifəsini aç                    |                         | login səhifəsi açılmalıdır           | login səhifəsi açıldı |
|2     | Email sahəsinə  invalid email  daxil et |  perH1234@gmail.com     |məlumat email sahəsində görünməlidir   |  email düzgün xanada görünür |
|3     | Password sahəsinə invalid şifrə daxil et|  M1237#qa               |şifrə password xanasında görünməlidir  |password düzgün xanada görünür  |
|4     |Login düyməsinə click et                 |                         |İstifadəçi sistemə daxil olmamalıdır   |"Daxil etdiyiniz Email və ya şifrə yanlışdır" xəta mesajı gəlir|

## TEST CASE 3
## TEST CASE ID : TC_003
## TITLE : Boş email və şifrə ilə Login funksiyasının yoxlanışı
## Precendition : Login səhifəsi açıqdır
|STEPS|   ACTION                   | DATA  |   EXPECTED  RESULT                             |  ACTUAL  RESULT                            |
|-----|----------------------------|-------|------------------------------------------------|--------------------------------------------|
|1    |Email sahəsini boş saxla    |       |Email xanasında heçnə yazılmamalıdır            |Email sahəsi boşdur                         |
|2    |Password  sahəsini boş saxla|       |Şifrə sahəsi boş olmalıdır                      |Password sahəsi boşdur                      |
|3    |"login " düyməsini clicklə  |       |Xəta mesajı çıxmalıdır və login baş verməməlidir| "Please fill out this field" mesajı gəlir  |


## Test Case 4
## Test Case ID : TC_004
## TITLE:Uğurlu  pul  köçurmə  əməliyyatı
## Precondition : Istifadəçi login  olmuşdur və hesabda kifayət qədər  balans var

| STEPS| ACTION                         |  DATA              | EXPECTED RESULT                                                    | ACTUAL RESULT                    
|------|--------------------------------|--------------------|-------------------------------------------------------------------  |-----------------------------|
|1     |Kapital Bank veb tətbiqini aç|                    | veb tətbiqin Home page görünməlidir                                    | Dashboard açıldı                   
|2     |"Pul köçürmə " bölməsinə keç |                    | Pul köçürmə səhifəsi açılmalıdır                                       |pul köçürmə səhifəsi açıldı                    
|3     | Kart nömrəsini daxil et     |1234 5678 9768 1090 |Kart nömrəsi xanada görunməlidir                                        |kart nömrəsi xanada görünür         
|4     | Köçürmə məbləği daxil et    | 50 AZN             | Daxil edilən məbləğ xanada görünməlidir                                |Köçürmə məbləği xanada görünür|
|5     | "Köçür" düyməsinə click et  |                    |əməliyyatın icrası başlamalıdır                                         | Prosses başlayır            |
|6     |Əməliyyatı təstiqlə          |                    | Pul uğurla köçürülür "Əməliyyat uğurla tamamlandı" mesajı göstərilməlidir|Köçürmə uğurla tamamlandı və təstiq mesajı gəldi     
                                                                           
## TEST CASE 5
## TEST CASE ID: TC_005
## TITLE : Balansdan artıq məbləğin köçürülməsi
## PRECONDITION :İstifadəçi login olmuşdur və  hesab balansı köçürülən məbləğdən azdır(Balans 500 AZN)

|STEPS| ACTION                          |DATA               | EXPECTED RESULT                   | ACTUAL RESULT                                 |
|-----|---------------------------------|-------------------|-----------------------------------|-----------------------------------------------|
|1    |Kapital bank tətbiqini aç        |                   | Tətbiq açılmalıdır                |Tətbiq açılır və home page görünür             |
|2    |Pul köçürmə səhifəsinə keç       |                   | Köçürmə səhifəsinə daxil olmalıdır| Pul köçürmə səhifəsi açılır                   |
|3    |Kart nömrəsini daxil et          |1997 2026 2021 1992| Nömrə uyğün xanada görünməlidir   |Kart nömrəsi düzgün xanada görünür             |
|4    |balansdan yuksək məbləğ daxil et |800 AZN            |məbləğ uyğun xanada görünməlidir   |Məbləğ düzgün xanada görünür                   |
|5    |Köçür düyməsinə click et         |                   |Xəbərdarlıq mesajı gəlməlidir      | Balans kifayət deyil xəbərdarlıq mesajı gəlir |






                  

