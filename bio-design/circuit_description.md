# Genetik Devre Tasarımı: BioSentez v1.0

## 🧬 Devre Mantığı (Logic)

Bu genetik devre, **Heavy Metal Sensing (Ağır Metal Algılama)** ve **Bioplastic Production (Biyoplastik Üretimi)** modüllerini entegre eder.

### 1. Algılama Modülü (Sensing)
*   **Promoter:** `P_zntA` (Çinko/Kadmiyum/Kurşun varlığında aktive olur).
*   **Regülatör:** `ZntR` (Ağır metal bağlandığında promoter'ı açar).
*   **Çıktı:** `Metallothionein` (MT) proteininin ekspresyonu için sinyal başlatır.
    *   *İşlev:* MT, hücre yüzeyinde ağır metalleri şelatlar (tutar).

### 2. Üretim Modülü (Production)
*   **Promoter:** `P_lac` (IPTG indüklenebilir veya konstitütif bir promoter ile değiştirilebilir).
*   **Operon:** `phaCAB` (Biyoplastik sentez yolağı enzimleri).
    *   `phaA`: 3-ketotiolaz
    *   `phaB`: Asetoasetil-CoA redüktaz
    *   `phaC`: PHA sentaz
*   **Terminator:** `T_rrnB` (Transkripsiyonu sonlandırır).

## 🔗 Entegrasyon
Ağır metal stresi, hücrenin metal tutma kapasitesini artırırken, eşzamanlı olarak (veya iki fazlı bir sistemle) karbon kaynağının plastiğe dönüşmesini sağlar.

## 🛠 Kullanılan Parçalar (BioBricks)
*   BBa_K123456 (Örnek)
*   BBa_J23100 (Konstitütif Promoter)
