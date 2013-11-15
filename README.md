Emlak Script
===========

<h5>Yayınlanan Son Kararlı Sürüm: 1.0 (08.11.2013)</h5>


Kurulum Yönergeleri
-----------

<ul>
  <li>Tüm dosyaları ftp ile sunucuya yükleyiniz</li>
  <li>Hosting panelinizden bir mysql veritabanı oluşturup, <b>veritabani.sql</b> dosyasını import edin</li>
  <li><b>protected/config/main.php</b> dosyasında yapılacak değişiklikler;
    <ul>
      <li>En üst bölümde bulunan <b>'name'</b> bölümüne web siteniz için bir isim yazın. Bu bazı sayfa başlıklarında ve metinlerde görünecektir.</li>
      <li><b>'db'</b> altındaki <b>'connectionString', 'username' ve 'password'</b> alanlarını oluşturduğunuz veritabanına göre düzenleyin.</li>
      <li>Eğer payPal sistemini kullanacaksanız, bir payPal hesabı alın ve api sistemini aktif edin. Ardından <b>'Paypal'</b> bölümü altındaki verileri kendinize göre düzenleyin.</li>
      <li>Sistemin mail göndermek için kullandığı ayarları <b>'Smtpmail'</b> bölümünden düzenleyin.</li>
    </ul>
  </li>
  <li><b>Yazma izni</b> verilecek klasörler;
    <ul>
      <li><b>/uploads</b></li>
      <li><b>/assets</b></li>
      <li><b>/images/ilan</b></li>
      <li><b>/images/magaza</b></li>
      <li><b>/images/slider</b></li>
      <li><b>/protected/runtime</b></li>
    </ul>
  </li>
</ul>

Yukarıdaki yönergeler sistemin sağlıklı çalışabilmesi için yeterlidir. Ancak profesyonel bir kullanıcı yada programcı iseniz <b>caching, url routing, error log</b> gibi bileşenleri de değiştirerek kendinize en uygun konfigürasyonu elde edebilirsiniz.

Hata Bildirimi
-----------
Hata yönetimi işlemleri de bu platformdan yürütülecektir. Sağ tarafta bulunan <b>issues</b> alanından hata bildirimi yapabilirsiniz. Bildiriler çoğunlukla aynı gün içinde değerlendirilecektir.


Sistem Gereksinimleri
-----------
Platform Yii framework kullanılarak inşa edildiği için framework'un gerektirdiği bazı bileşen ve değerler vardır. Bunlar zorunlu ve önerilen olarak 2 bölümde bildirilmiştir;

<h4>Zorunlu olan gereksinimler</h4>
Günümüz birçok sunucusu zaten aşağıda belirtilen gereksinimleri karşılamaktadır. Ancak ortak bir sunucu(hosting) kullanıyorsanız tüm bileşenler kurulu olmayabilir. Bunun için lütfen sunucu yöneticisine danışın.
<ul>
  <li>PHP sürümü 5.1.0 ve üstü olmalıdır</li>
  <li>$_SERVER değişkeni kullanılabilir olmalıdır</li>
  <li>safe_mode pasif(off) olmalıdır.</li>
  <li>Reflection eklentisi</li>
  <li>PCRE eklentisi</li>
  <li>SPL eklentisi</li>
  <li>DOM eklentisi</li>
  <li>PDO eklentisi</li>
  <li>PDO MySQL eklentisi</li>
  <li>PDO SQLite eklentisi</li>
  <li>SOAP eklentisi</li>
  <li>GD eklentisi</li>
  <li>ionCube eklentisi</li>
</ul>

<h4>Önerilen bileşenler</h4>
<ul>
  <li>APC eklentisi (cache sistemidir. Kesinlikle önerilmektedir. %70'e kadar bir performans artışı sağlar)</li>
  <li>Memcache eklentisi (APC istemiyorsanız ve farklı 2 sunucu kullanmak isterseniz yüksek performans sağlar)</li>
</ul>

<h4>Sorumluluklar</h4>
Sistemde meydana gelebilecek herhangi bir problem yada güvenlik açığı gibi sebeplerden dolayı oluşabilecek zarardan ancak script'i kullanan kurum/şahıs kendisi sorumludur.
