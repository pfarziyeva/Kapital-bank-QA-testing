## Test Case 1
## Test Case ID:TC_001
## Title:Valid məlumatlarla Login fünksiyasının yoxlanışı
## Preconditions: İstifadəçi  sistemdə  qeydiyyatdan  keçib

|steps|   Action               |    Data              |    Expected Result                                   |    Actual Rsult      |
|-----|------------------------|----------------------|------------------------------------------------------|----------------------|
|1    |  Saytı aç              |                      |  Kapital bank veb saytı açılır                       |    Sayt açılır       |                      
|2    |Login səhifəsini aç     |                      |  Səhifə açılır                                       |
|3    |Valid  email daxil et   | pervinferzi@gmail.com| məlumat email sahəsində görünür                      |                      |
|4    |Valid password daxil et | H1234%miko           |  password şifrə sahəsində görünür                    |                                
|5    |Login düyməsinə click et|                      | Istifadəçi girişi uğurlu olur.Profil səhifəsi açılır |                      |


## Test case 2
## Test case ID: TC_002
## Title: Invalid məlumatlarla Login funksiyasının yoxlanışı
## Precondition:Qeydiyyatdan keçmiş istifadəçi mövcüddür


