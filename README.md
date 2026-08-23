# YKS Veri

**https://yks.oguzergin.net**

2018-2026 arasında Türkiye'de üniversiteye yerleştirmenin ne olduğunu gösteren
durağan bir sayfa. Bütün sayılar ÖSYM, YÖK Atlas ve Sağlık Bakanlığı'nın kamuya
açık yayınlarından kendi ayrıştırmamızla üretildi.

Hazırlayan: Prof. Dr. Oğuz Ergin · [oguzergin.net](https://oguzergin.net)

## Sayfada ne var

1. **İlk 100 program** · her yıl en yüksek tabanlı 100 programın bölüm dağılımı, üç puan türü
2. **Program mı, koltuk mu** · aynı listenin kontenjanla ağırlıklandırılmış hâli
3. **Üniversiteler yer değiştirdi mi** · bölüm bölüm ilk 20, dokuz yıllık çizgi
4. **Başarı sırası çizelgeleri** · sekiz bölüm için program program sıra serisi
5. **Bölüm bölüm üniversiteler** · 34 bölümde kurumların bölüm içi yüzdeliği
6. **Yükselen ve düşen bölümler** · dokuz yıllık zincirleme endeks
7. **Tıp** · kontenjan ve ilk sıraların dağılımı
8. **Haritalar** · il il tıp kontenjanı, tıp taban sırası, hekim sayısı, 100 binde hekim
9. **Yöntem ve kaynaklar**

## Kaynaklar

| veri | kaynak | yıl |
|---|---|---|
| Kontenjan, yerleşen, taban puan | ÖSYM Tablo-4 merkezi yerleştirme sonuçları | 2018-2026 |
| Başarı sırası | ÖSYM tercih kılavuzu Tablo-4, "bir önceki yıl başarı sırası" sütunu | 2018-2025 |
| Başarı sırası | YÖK Atlas | 2026 |
| Hekim sayısı ve nüfus | Sağlık Bakanlığı, Sağlık İstatistikleri Yıllığı 2024, Tablo 10.12 ve 1.3 | 2024 |
| İl sınırları | datamaps TopoJSON | |

## Üç yöntem kuralı

**Başarı sırası aday havuzuna bölünmez.** Öğrenciler en tepeden tercih yapıyor;
alta aday eklenmesi mutlak sıralamayı etkilemiyor. Havuza bölmek, aday sayısı
artan puan türlerinde sahte iyileşme üretiyor.

**Sıra serileri aynı program kodunun yıl yıl eşleştirilmesiyle kuruluyor.** Her
ardışık yıl çifti ayrı eşleştiriliyor, ortanca oranlar çarpılıyor. Tek atlamayla
ölçmek eşleşmeyi çok daraltıyor.

**Dolmayan programa ÖSYM sıra atamıyor** ve bu eksiklik rastgele değil, zayıf
programlarda yoğunlaşıyor. Sıra ölçütü kullanılan her yerde kapsam ayrıca veriliyor.

Ayrıntılı yöntem sayfanın 9. bölümünde.

## Bu depoda ne yok

- **Ham veri yok.** ÖSYM ve Sağlık Bakanlığı dosyaları kaynak kurumların kendi
  sitelerinde; buraya kopyalanmadı.
- **Kişisel veri yok ve hiçbir zaman olmayacak.** Depoya kopyalayan betik her
  çalıştırmada tablo dosyası ve kişisel veri izi arayıp bulursa duruyor.
- **Betikler burada değil.** Sayfayı üreten Python betikleri ayrı bir çalışma
  ağacında duruyor; bu depo yalnız yayımlanan çıktıyı taşıyor.

## Teknik

Tamamen durağan. Dışarıdan hiçbir betik, yazı tipi ya da görsel yüklenmiyor;
çevrimdışı da açılıyor. Çizelgeler ve haritalar PNG olarak gömülmedi, JSON'dan
tarayıcıda SVG olarak çiziliyor. Gerekçesi pratik: **yayımlanmış görsel donuyor,
sayfa düzeltilebiliyor.** Paylaşım için gereken PNG'ler `gorsel/` altında duruyor
ve her bölümün altında indirme bağlantısı var.

Açık ve koyu tema, telefonda yatay kaydırma yok.

## Kullanım

Sayılar kamuya açık resmî yayınlardan türetildi. Alıntılarken kaynak olarak hem
bu sayfayı hem ilgili kurumu (ÖSYM, YÖK, Sağlık Bakanlığı) belirtin.
