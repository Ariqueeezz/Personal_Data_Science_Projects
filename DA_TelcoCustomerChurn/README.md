# 📡 Telco Customer Churn Analysis & Retention Strategy

![Project Status](https://img.shields.io/badge/Status-Completed-success)
![Tools](https://img.shields.io/badge/Tools-Python%20%7C%20Looker%20Studio-blue)
![Domain](https://img.shields.io/badge/Domain-Telecommunication-orange)

> **"Stopping the bleeding before it becomes a hemorrhage."**
> Analisis end-to-end untuk mendeteksi akar penyebab *churn* dan merumuskan strategi retensi berbasis data guna mengamankan pendapatan perusahaan di Q4.

---

## 👤 Author
**Raihan Ariq Muzakki**
*Data Analyst Portfolio*

---

## 📑 Table of Contents
- [Latar Belakang & Masalah Bisnis](#-latar-belakang--masalah-bisnis)
- [Data Overview](#-data-overview)
- [Diagnosa & Insight Kunci](#-diagnosa--insight-kunci)
- [Dashboard Monitoring](#-dashboard-monitoring)
- [Rekomendasi Bisnis (Solusi)](#-rekomendasi-bisnis-solusi)
- [Struktur Proyek](#-struktur-proyek)

---

## 💼 Latar Belakang & Masalah Bisnis

### 📉 Situasi: Industri yang "Berdarah-darah"
Industri telekomunikasi sedang menghadapi persaingan yang brutal. Kompetitor agresif menawarkan perangkat canggih dan harga miring, membuat loyalitas pelanggan sangat rapuh.

### ⚠️ Masalah Utama
Perusahaan kehilangan pelanggan setia **bukan karena produk mati total**, melainkan karena:
1.  **Masalah Operasional:** Kualitas modem usang & layanan teknisi yang kurang ramah.
2.  **Serangan Kompetitor:** Penawaran harga dan perangkat yang lebih baik.

### 🔥 Urgensi (The Risk)
Menuju **Kuartal 4 (Q4)** masa "perang promo" akhir tahun—risiko kebocoran pendapatan (*Revenue Loss*) diprediksi meningkat drastis. Proyek ini bertujuan untuk mendiagnosa siapa yang akan pergi dan apa obatnya sebelum terlambat.

---

## 💾 Data Overview

**Sumber Data:** IBM Cognos Analytics - Telecommunication Industry Sample Data.  
**Volume:** 7,043 Profil Pelanggan | 33 Fitur.

Dataset mencakup pandangan 360-derajat pelanggan:
* **Demografi:** Gender, Senior Citizen, Pasangan, Tanggungan.
* **Layanan:** Telepon, Internet, Streaming, Dukungan Teknis.
* **Akun:** Tenur, Kontrak, Metode Pembayaran, Tagihan Bulanan.
* **Lokasi:** Negara Bagian, Kota (California), Kode Pos.

---

## 🔎 Diagnosa & Insight Kunci

Berdasarkan analisis data mendalam, ditemukan 3 fakta kritis:

### 1. Geographic Hotspot: "Anomali San Diego" 📍
Terdapat konsentrasi *churn* yang ekstrim di wilayah San Diego.
* **Fakta:** San Diego menyumbang **185 pelanggan churn**, lebih dari 2x lipat dibandingkan Los Angeles.
* **Analisis:** Ini mengindikasikan serangan kompetitor lokal atau masalah infrastruktur spesifik di area tersebut, bukan kegagalan nasional.

### 2. Akar Masalah: Perang Harga & Perangkat 💸
Menggunakan Prinsip Pareto (80/20), mayoritas alasan pelanggan pergi didominasi oleh faktor komersial.
* **Fakta:** Alasan tertinggi adalah **"Competitor made better offer"** dan **"Competitor had better devices"**.
* **Analisis:** Pelanggan sebenarnya puas dengan sinyal (*Network Reliability* bukan isu utama), namun mereka kalah dalam perang harga.

### 3. Segmen Risiko Tinggi: Lansia & Pelanggan Baru ⚠️
* **Senior Citizen:** Tingkat churn mencapai **25.5%** (2x lipat dari non-lansia), menandakan layanan yang kurang ramah lansia.
* **Zona Bahaya:** Risiko tertinggi ada di **6 bulan pertama** (*Onboarding*).

---

## 📊 Dashboard Monitoring

**"Customer Retention Command Center"**
Dashboard interaktif berbasis Looker Studio dirancang untuk memantau risiko secara real-time.

**Fitur Utama:**
* **Peta Risiko Geografis:** Memantau titik panas *churn* (fokus San Diego).
* **Matriks Prioritas:** Mengelompokkan pelanggan menjadi *Champions* vs *Vulnerable*.
* **Actionable List:** Daftar target prioritas untuk tim marketing.

![Dashboard Preview](/DA_TelcoCustomerChurn/TelcoCustChurnDashboard.jpg)

---

## 💡 Rekomendasi Bisnis (Solusi)

Strategi konkret untuk menyelamatkan Revenue Q4:

### 🛡️ 1. Operation San Diego (Localized Strategy)
* **Taktik:** Luncurkan promo *"San Diego Exclusive Deal"* dan program *Free Modem Upgrade* khusus di kode pos San Diego.
* **Tujuan:** Melawan dominasi penawaran kompetitor secara spesifik di wilayah terdampak.

### 👵 2. Program "Silver Service"
* **Taktik:** Jalur layanan prioritas (*Direct Human*) untuk Lansia dan penyederhanaan tagihan.
* **Tujuan:** Menurunkan *churn rate* segmen Lansia dengan pendekatan personal (*High-Touch*).

### 💰 3. The Pareto Opportunity
* **Taktik:** Alokasikan anggaran retensi terbesar untuk melawan **"Competitor Offers"** (Subsidi harga).
* **Dampak:** Solusi paling efisien karena menangani penyebab utama (80% masalah) dengan satu fokus strategi.

---

## 📂 Struktur Proyek

```bash
DA_TelcoCustomerChurn/
├── 📄 README.md                   # Dokumentasi Proyek
├── 📓 TelcoChurn_Notebook.ipynb      # Notebook Analisis (Cleaning, EDA, Visualisasi)
├── 📊 PS 16-Raihan Ariq Muzakki.pdf # File Presentasi Analisis
└── 📄 dataset/                       # File Dataset
```

## 🛠 Tools
- **Python**: Pandas, Matplotlib, Seaborn (Analisis & EDA).

- **Looker Studio**: Visualisasi & Dashboard Interaktif.

- **Google Colab Notebook**: Environment Analisis.