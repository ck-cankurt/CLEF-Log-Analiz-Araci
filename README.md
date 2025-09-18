# CLEF Log Analiz Aracı

## 📋 Proje Hakkında

CLEF Log Analiz Aracı, CLEF (Compact Log Event Format) formatındaki log dosyalarını analiz eden ve hataları görselleştiren web tabanlı bir araçtır. Büyük log dosyalarında hataları hızlıca bulmanızı, filtrelemenizi ve analiz etmenizi sağlar.

<img width="1264" height="512" alt="image" src="https://github.com/user-attachments/assets/4bf02d38-ca4a-4f95-bab5-53eed2506663" />


## ✨ Özellikler

- **📁 Dosya Yükleme**: CLEF, LOG veya TXT formatındaki dosyaları destekler
- **🔍 Akıllı Hata Tespiti**: Log dosyalarındaki hataları otomatik olarak algılar ve kategorize eder
- **📊 İstatistikler**: Toplam hata sayısı, hata türü dağılımı ve zaman aralığı istatistikleri
- **🎯 Gelişmiş Filtreleme**: 
  - Hata türüne göre filtreleme
  - İşlem türüne göre filtreleme
  - Metin arama ile filtreleme
- **📍 Detaylı Hata Bilgisi**: Her hata için dosya konumu, satır numarası ve method çağrı zinciri
- **🎨 Kullanıcı Dostu Arayüz**: Modern ve responsive tasarım

<img width="1188" height="891" alt="image" src="https://github.com/user-attachments/assets/b113e070-cbb7-4b64-b995-154d0508468a" />


## 🚀 Kullanım

1. Tarayıcınızda HTML dosyasını açın
2. "Log Dosyası Seçin" butonuna tıklayarak CLEF formatındaki log dosyanızı yükleyin
3. "Hata Analitiğini Çalıştır" butonuna tıklayın
4. Analiz sonuçlarını inceleyin ve gerekirse filtreleri kullanarak arama yapın

## 🔧 Desteklenen Hata Türleri

- Bellek Hataları (OutOfMemoryException)
- Taşma Hataları (OverflowException)
- Parametre Hataları (ArgumentException)
- Null Referans Hataları (NullReferenceException)
- Geçersiz İşlem Hataları (InvalidOperationException)
- Zaman Aşımı Hataları (TimeoutException)
- Veritabanı Hataları (SqlException)
- HTTP İstek Hataları (HttpRequestException)
- Yetki Hataları (UnauthorizedAccessException)
- Dosya/Dizin Hataları
- Ağ Hataları
- Ve daha fazlası...

## 💡 Özellik Detayları

### Akıllı İşlem Türü Tespiti
Uygulama, log mesajlarından ve exception stack trace'lerinden otomatik olarak işlem türünü tespit eder:
- Sipariş işlemleri (Satınalma, Satış)
- Transfer işlemleri (Cari, Stok, Fason)
- Veri işlemleri (İçe/Dışa Aktarma)
- Sistem işlemleri (Yedekleme, Senkronizasyon, Konfigürasyon)

### Stack Trace Analizi
Her hata için detaylı method çağrı zinciri gösterilir:
- Hatanın oluştuğu dosya ve satır numarası
- Method çağrı sırası
- Genişletilebilir stack trace görünümü

## 🛠️ Teknik Detaylar

- **Teknoloji**: Vanilla JavaScript, HTML5, CSS3
- **Format**: CLEF (Compact Log Event Format) JSON yapısı
- **Tarayıcı Desteği**: Modern tarayıcılar (Chrome, Firefox, Edge, Safari)
- **Bağımlılık**: Yok (standalone uygulama)

## 📝 CLEF Format Örneği
```json
{"@t":"2024-01-15T10:30:45.123Z","@l":"Error","@mt":"Hata mesajı","@x":"Exception detayları..."}
```
## 🎯 Kullanım Senaryoları

- Üretim ortamındaki hataların hızlı analizi
- Geliştirme sürecinde debug işlemleri
- Sistem performans sorunlarının tespiti
- Hata trendlerinin takibi
- Kritik hataların önceliklendirilmesi

## 📌 Notlar

- Büyük log dosyaları (100MB+) için performans optimizasyonu yapılmıştır
- Tüm işlemler tarayıcı üzerinde gerçekleşir, veriler sunucuya gönderilmez
- Dosya içeriği bellekte işlenir ve sayfa yenilendiğinde temizlenir

## 🤝 Katkıda Bulunma
- Pull request'ler kabul edilir. Büyük değişiklikler için lütfen önce bir issue açın.

##📄 Lisans
- Bu proje açık kaynaklıdır ve sadece FORK kullanımı serbesttir. https://github.com/ck-cankurt/
