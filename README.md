# SmartEnergyBuddy
# 🚀 SmartEnergy - Akıllı Enerji İzleme ve Kestirimci Bakım Sistemi

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0+-orange.svg)
![Azure](https://img.shields.io/badge/Azure-IoT%20Hub-0089D6.svg)
![Docker](https://img.shields.io/badge/Docker-Enabled-2496ED.svg)

**Endüstriyel makineler için gerçek zamanlı enerji izleme ve arıza tahmin sistemi**

</div>

## 📋 Proje Özeti

SmartEnergy, fabrika ve endüstriyel tesislerdeki makinelerin enerji tüketimini izleyen, anormal durumları tespit eden ve arıza riskini önceden tahmin eden kapsamlı bir IoT çözümüdür. Proje endüstriyel otomasyon standartlarına uygun olarak geliştirilmiştir.

### 🎯 Temel Özellikler

- 🔍 **Gerçek Zamanlı İzleme**: Enerji tüketimi, sıcaklık, titreşim verileri
- 🤖 **AI Destekli Tahmin**: LSTM ve Random Forest ile arıza öngörüsü
- ⚡ **Edge Computing**: Raspberry Pi üzerinde yerel işlem
- ☁️ **Bulut Entegrasyonu**: Azure IoT Hub ile merkezi yönetim
- 📊 **Canlı Dashboard**: Grafana/Power BI ile görselleştirme
- 🔒 **Endüstriyel Güvenlik**: TLS/SSL şifreleme ve erişim kontrolü

## 🏗️ Sistem Mimarisi
Katman 1: Veri Kaynakları → Simüle sensörler (OPC UA/MQTT)
Katman 2: Edge İşleme → Raspberry Pi + Docker + Python
Katman 3: AI Modülü → TensorFlow/Scikit-learn modelleri
Katman 4: Bulut Entegrasyon → Azure IoT Hub
Katman 5: Görselleştirme → Grafana Dashboard
Katman 6: Güvenlik → TLS/SSL + API Token


## 🛠️ Teknoloji Stack'i

| Bileşen | Teknolojiler |
|---------|--------------|
| **Programlama** | Python, C++, Node-RED |
| **AI/ML** | Scikit-learn, TensorFlow, Pandas, NumPy |
| **Edge Computing** | Raspberry Pi, Docker, Docker Compose |
| **IoT Protokolleri** | MQTT, OPC UA, Modbus |
| **Bulut** | Azure IoT Hub, AWS IoT Core |
| **Görselleştirme** | Grafana, Power BI |
| **Veritabanı** | InfluxDB, PostgreSQL |
| **Güvenlik** | TLS/SSL, JWT Token |

## 📦 Kurulum

### Ön Koşullar
- Python 3.8+
- Docker & Docker Compose
- Azure IoT Hub hesabı (opsiyonel)

### Hızlı Başlangıç

1. **Repository'yi klonlayın:**
```bash
git clone https://github.com/your-username/smart-energy-monitoring.git
cd smart-energy-monitoring
```

Gerekli paketleri yükleyin:
```bash
pip install -r requirements.txt
```

AI modellerini eğitin:

```bash
cd notebooks
jupyter notebook model_training.ipynb
```


Edge servislerini başlatın:
```bash
cd edge
docker-compose up -d
```

Dashboard'u başlatın:

```bash
cd dashboard
docker-compose up -d
```

🚀 Kullanım
Veri Simülasyonu
```
bash
python scripts/simulate_sensors.py --duration 3600 --interval 5
```

Model Inference
```
bash
python edge/edge_inference.py --model models/failure_predictor.pkl
```
Dashboard Erişimi
Grafana: http://localhost:3000

Node-RED: http://localhost:1880

📁 Proje Yapısı

smart-energy-monitoring/
├── data/                 # Veri setleri ve simülasyon verileri
├── notebooks/           # Jupyter notebook'ları (EDA ve model eğitimi)
├── edge/               # Edge computing bileşenleri
├── cloud/              # Bulut entegrasyon kodları
├── dashboard/          # Görselleştirme ve dashboard'lar
├── models/             # Eğitilmiş AI modelleri
├── scripts/            # Yardımcı script'ler
├── docs/               # Dokümantasyon
└── tests/              # Test dosyaları

🤝 Katkıda Bulunma
- Fork edin
- Feature branch oluşturun (git checkout -b feature/amazing-feature)
- Commit edin (git commit -m 'Add amazing feature')
- Push edin (git push origin feature/amazing-feature)
- Pull Request oluşturun

📄 Lisans
Bu proje MIT lisansı altında lisanslanmıştır - detaylar için LICENSE dosyasına bakın.

👩‍💻 Geliştirici
Damla - Bilgisayar Mühendisliği Öğrencisi

📧 E-posta: damlanuralper20@gmail.com.com

💼 LinkedIn: LinkedIn Profili

🐙 GitHub: GitHub Profili


<div align="center">
⭐ Bu projeyi beğendiyseniz yıldız vermeyi unutmayın!

</div> ```
