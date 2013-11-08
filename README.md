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
