# İş Analizi ve Süreç Tasarımı Vaka Çalışması: Paynet & ttec

## Proje Özeti
Bu proje, 30.000'den fazla işletmenin finansal süreçlerini dijitalleştiren ve Merkez Bankası lisanslı bir finansal teknoloji şirketi olan Paynet'in ödeme sistemleri altyapısı üzerinden gerçekleştirilmiş bir iş analizi vaka çalışmasıdır. Çalışma kapsamında 'ttec' firmasının satış süreçleri incelenmiş ve müşteri deneyimini iyileştirmeye yönelik sistem gereksinimleri analiz edilmiştir.

## İş Hedefi ve Problem Tanımı
*   **Problem:** ttec web sitesinin sepet sayfasındaki algoritmanın önerdiği ürünlerin sepete eklenme oranının %5 gibi düşük bir oranda kalması. Mevcut siparişlerden elde edilen verilerin, tüketici davranışlarını anlamakta yetersiz kalması.
*   **Çözüm ve Hedef:** Ödeme sayfasında (Sanal POS adımı) müşterilerden yaş, eğitim durumu, medeni hal, teknolojik harcamalara ayrılan bütçe ve hobiler gibi demografik verilerin toplanması. Bu sayede kullanıcıların sınıflandırılarak doğru kişiye doğru ürünün (örneğin evli müşterilere elektrikli süpürge) önerilmesi ve satış hacminin artırılması hedeflenmiştir.

## Kullanıcı Hikayeleri (User Stories)
Projedeki gereksinimler iki farklı paydaş perspektifinden ele alınmıştır:
*   **Dış Paydaş (Müşteri):** "Bir müşteri olarak online ürün satın almak istiyorum. Böylelikle kolay ve hızlı bir şekilde ürünlerime ulaşmak istiyorum."
*   **İç Paydaş (Ürün ve Satış Yöneticisi):** "Bir Ürün ve Satış Yöneticisi olarak müşterilerden kişisel verilerini talep etmek istiyorum, böylelikle kişiselleştirilmiş bir hizmet sunabileceğim."

## Süreç Akışı ve Kabul Kriterleri (Acceptance Criteria)
Ürünün sepete eklenmesinden ödemenin tamamlanmasına kadar geçen ana akış (Main Flow) tasarlanmış ve oluşabilecek istisnai durumlar (Exceptions) belirlenmiştir. Sistem akışındaki hataları önlemek adına GIVEN-WHEN-THEN formatında 10 farklı senaryo oluşturulmuştur. Bu senaryolardan bazıları şunlardır:
1.  Satın alınmak istenen ürünün stoğunun olmaması.
2.  Eksik, hatalı veya onaysız kredi kartı girişi yapılması.
3.  Zorunlu alanların (TCKN vb.) boş bırakılması veya hatalı girilmesi.
4.  Güvenlik kodunun (SMS) gelmemesi veya süresinin dolması.
5.  Kartta yeterli bakiyenin bulunmaması.

## Dokümantasyon ve Çıktılar
Bu depoda yer alan proje dokümanı (PDF) içerisinde detaylı gereksinim analizine ek olarak aşağıdaki süreç tasarım çıktıları bulunmaktadır:
*   **İş Akış Diyagramı:** Kullanıcı kararları ve sistem döngülerini içeren akış şeması.
*   **Ekran Tasarımları (Wireframes):** Giriş, Hesap Oluşturma, Adres Ekleme ve anket kutucuklarını (radio button, drop down, text area) barındıran Ödeme Ekranı tasarımları.
*   **Test Senaryosu Tablosu:** Stok, üyelik, TCKN, SMS ve bakiye gibi parametrelerin farklı varyasyonlarıyla oluşturulan uçtan uca test durumları.
