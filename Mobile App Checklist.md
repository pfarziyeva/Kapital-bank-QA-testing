# Mobile  Banking App  Testing  Checklist
## Installation testing
- ### Tətbiq  Google  Play və  ya  App  Store-dan  düzgün  yüklənir
- ### Tətbiq  uğurla quraşdırılır
- ### Quraşdırma  tamalandıqdan  sonra tətbiqin  ikonu cihaz  menyüsünda düzgün görünür.
- ### Tətbiq  açıldıqda ilkin  səhifə  düzgün  yüklənir.
- ### Tətbiq  uninstall  ediləndə  düzgün  silinir
- ### Tətbiqin yenidən  quraşdırılması zamanı hər  hansı   məlumat  itkisi və  ya texniki  problem yaranmır.
  
  ## Application  Launch / Splash Screen  Testing
  
- ### Tətbiq  ikonuna  click edildikdə tətbiq  düzgün  açılır.
- ### Tətbiq  açılan zaman Splash Screen düzgün  göstərilir.
- ### Splash Screen üzərində  tətbiqin loqosu  və dizayn elementləri düzgün görünür. 
- ### Tətbiqin  açılma   müddəti  qəbul edilən performans  limitləri daxilindədir.
- ### Tətbiq açılış  zamanı  donmur  və  crash  vermir.

  ## Login / Authentication Testing
  - ### Düzgün  username  və password ilə sistemə  uğurlu  giriş mümkün  olur.
  - ### Yanlış username və şifrə  daxil  edildikdə " İnvalid username  or  password " xəta mesajı  göstərilir
  - ### İstifadəçi  adı və ya şifrə  sahəsi  boş saxlanıldıqda  "  Please fill in all required fields " xəta  mesajı  görünür .
  - ### Şifrə minimum limitdən yəni 8 simvoldan az olduqda  xəbərdarlıq mesajı gəlir
  - ### Şifrədə hərf, rəqəm  və xüsüsi simvolların istifadəsi  mümkündür
  - ### Şifrə maskalanmsı fünksiyası düzgün işləyir
  - ### Forgot password  fünksiyası düzgün icra olunur.
 
    ## UI / UX testing
  - ### Tətbiq  interfeysində  bütün elementlər düzgün  görünür.
  - ### Mətnlər oxunaqlı  və düzgün  formatda  göstərilir.
  - ### Font və  iconlar  düzgün  görünür
  - ### Ekran elementləri  bir-birinin  üzərinə  düşmür
  - ### Scrool fünksiyası düzgün  işləyir.
  - ### Düymələr  və  linklər düzgün səhifəyə yönləndirir.
  - ### Landscape və Portrait rejimlərində  ekran  elementlərinin  görünüşü  düzgündür.

   ## Navigation  Testing
  - ### Tətbiq  daxilində  səhifələr  arasında keçid  düzgün  işləyir
  - ### Back düyməsi  düzgün işləyir
  - ### İstifadəçi  əsas  səhifəyə  rahat  qayıda  bilir.
  - ### Menü elementləri düzgün   yönləndirir.

   ## Network  Testing
   - ### Zəif  internet bağlantısında tətbiqin  davranışı yoxlanılır.
   - ### İnternet  bağlantısı  kəsildikdə yəni  offline  rejimdə "  You're  offline! Check your internet connection " xəta  mesajı gəlir.
   - ### internet  bərpa olunduqda  tətbiq  işləməyə  davam edir.
      
        
   ## Notification  Testing
        
   - ### Push notificationlar düzgün  göndərilir
   - ### Notification click  edildikdə uyğun  səhifə  açılır.
   - ### Notification  məzmunu  düzgün  göstərilir.

   ## Security  Testing
  - ### Şifrə  daxil  edilərkən məlumat gizli  şəkildə göstərilir  yəni  maskalnır.
  - ### İstifadəçi  sessiyası  müəyyən  müddətdən  sonra avtomatik  bağlanır.
  - ### Birdən  çox uğursuz  login  cəhdindən  sonra hesabın müvəqqəti bloklanması yoxlanılır.
  - ### Logout etdikdən sonra " Back buttonu " ilə hesab səhifəsinə daxil olmaq yoxlanılır.
  - ### Güclü şifrə tələbləri yəni böyük hərf , kiçik hərf ,rəqəm  və xüsüsi simvolların istifadəsi yoxlanılır.
  - ### Şifrə dəyişdirildikdən  sonra köhnə  şifrənin istifadə edilə bilməməsi yoxlanılır.
  - ### İstifadəçinin icazəsi olmayan səhifələrə daxil ola bilməməsi  yoxlanılır
  - ### Tətbiqin yalnız təhlükəsiz bağlantı yəni HTTPS protokolu istifadə etməsi yoxlanılır
  - ### Session token-ların təhlükəsiz ötürülməsi yoxlanılır.
  

    ## Transfer  Testing
    - ### Düzgün istifadəçi məlumatları ilə istənilən bank kartına transfer mümkündür.
    - ### Mənim kart hesablarım arasında pul köçürmə fünksiyası düzgündür
    - ### Balansdan artıq məbləğ daxil edildikdə " Insufficient balance.Please check your account balance. "  xəbərdarlıq mesajı görünür
    - ### Mənfi və ya sıfır  məbləğ sistem tərəfindən qəbul edilmir və xəbərdarlıq mesajı gəlir
    - ### Günlük transfer limiti aşıldıqda sistəmə xəbərdarlıq mesajı gəlir
    - ### Boş sahələrlə transfer mümkün olmur və " Please fill in all required fields" xəta mesajı görünür.
    - ### Minimum köçurmə məbləğindən aşağı məbləğ daxil edildikdə " Minimum köçürmə məbləği X AZN-dir " xəbərdarlıq mesajı görünür
    - ### Transferin təstiqi üçün OTP  və ya SMS kodunun göndərilməsi yoxlanılır
    - ### Yanlış OTP daxil  edildikdə xəta mesajının göndərilməsi  yoxlanılır.
    - ### OTP kodunun vaxt limiti yoxlanılır
    - ### Transferdən  sonra əməliyyatın history-də görünməsi yoxlanılır
    - ### Tarix məbləğ və alıcı  məlumatlarının düzgün  göstərilməsi yoxlanılır
      
    ## Compatiblity Testing
    - ### Tətbiqin muxtəlif mobil cihaz modellərində (müxtəlif ekran ölçüləri və hardware xüsüsiyyətləri  olan cihazlarda ) düzgün işləməsi  yoxlanılır
    - ### Tətbiqin müxtəlif operating system versiyalarında ( Android / İOS) stabil işləməsi yoxlanılır.
    - ### Tətbiqin müxtəlif ekran ölçülərində və resolution-larda UI  elementlərinin düzgün  görünməsi yoxlanılır
    - ### Tətbiqin portrait və landscape rejimlərində düzgün işləməsi  yoxlanılır
    - ### Tətbiqin müxtəlif istehsalçı cihazlarında ( Samsung, Xiaomi ,Huawei və s.) fünksional olaraq düzgün  işləməsi yoxlanılır
    















    
