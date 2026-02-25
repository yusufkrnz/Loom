# 🧵 Loom – Akıllı Sağlık Verisi Entegrasyon Gateway'i

## 🇹🇷 Türkçe Açıklama
**Loom**, standart dışı ve karmaşık sağlık verilerini (Legacy JSON, XML, String) dünya standardı olan **HL7 FHIR** formatına dönüştüren yüksek performanslı bir ara yazılımdır.  

Özellikler:
- **FastAPI tabanlı asenkron mimari**: Yüksek performanslı ve ölçeklenebilir veri işleme.  
- **Dinamik Mapping Motoru**: Veri alanlarını esnek bir şekilde eşler ve dönüştürür.  
- **Otomatik Tıbbi Terminoloji Eşleme (LOINC)**: Klinik terimleri standart kodlara çevirerek veriyi “konuşabilir” hâle getirir.  

> “Veri nereden gelirse gelsin, Loom onu standartlara dokur.”

---

## 🇺🇸 English Description
**Loom** is a high-performance middleware designed to transform non-standard, legacy healthcare data (JSON, XML, String) into globally recognized **HL7 FHIR** resources.  

Key Features:
- **FastAPI-driven asynchronous pipeline**: High-performance, scalable data processing.  
- **Dynamic Mapping Engine**: Flexibly maps and transforms data fields.  
- **Automated Medical Terminology Enrichment (LOINC)**: Converts clinical terms into standardized codes, making data “talkable.”  

> "No matter the source, Loom weaves your data into standards."

---

## 📌 Projenin Teknik Temeli
- **Decoupled Architecture** – Parser ve Validator birbirinden bağımsız, kolay güncellenebilir.  
- **Semantic Mapping Intelligence** – Veri anlamını korur ve uluslararası terminolojiye dönüştürür.  
- **Atomic Integrity** – İşlemler ya tamamen gerçekleşir ya iptal edilir; sağlık verisi tutarlılığı garanti edilir.

---

## 🚀 Başlangıç ve Kurulum
```bash
# Repo klonlama
git clone https://github.com/kullanici/loom.git
cd loom

# Sanal ortam oluşturma
python -m venv venv
source venv/bin/activate  # Linux / macOS
venv\Scripts\activate     # Windows

# Gereksinimleri yükleme
pip install -r requirements.txt

# Uygulamayı başlatma
uvicorn loom.main:app --reload
