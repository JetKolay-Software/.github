---
name: ✨ Kapsamlı Özellik / Sayfa İsteği
about: Yeni bir sayfa veya majör özellik geliştirmesi için detaylı şablon
title: "[FEAT] <Özellik Adı>"
labels: enhancement
assignees: ''
---

## 📋 Genel Bilgiler
| Özellik | Detay |
| :--- | :--- |
| **Öncelik** | `Yüksek` / `Orta` / `Düşük` |
| **Tahmini Efor** | `...` Gün |
| **İlgili Servisler** | `MP-Frontend`, `...-Service` |

## 📌 Özet
> Örn: Mükelleflerin tebligatlarını tek merkezden yönetebileceği arayüz...

---

## 🧭 Sayfa Yapısı ve Bileşenler

### 1. Üst Kontrol Paneli (Header Actions)
- **Buton 1:** `[İkon]` [Buton Adı]
  - **Davranış:** (Örn: Modal açılır, Excel indirir...)
  - **API Tetik:** (Varsa endpoint)

### 2. Filtreleme Alanı (Filter Bar)
- [ ] Tarih Aralığı (`alan_adi`)
- [ ] Dropdown Seçim (`alan_adi`)
- [ ] Text Arama (`alan_adi`)

### 3. Veri Tablosu (Data Grid)
| UI Sütun Başlığı | DB Alanı | Görünüm / Format | Notlar |
| :--- | :--- | :--- | :--- |
| Durum | `status` | Badge (🟢/🔴) | - |
| Belge No | `belge_no` | Text | - |
| Tarih | `created_at` | dd.MM.yyyy HH:mm | - |
| ... | ... | ... | ... |

**Tablo Özellikleri:**
- [ ] Server-side Pagination
- [ ] Sorting
- [ ] Multi-select Checkbox

### 4. Satır Aksiyonları (Row Actions)
- **Aksiyon 1:** `[İkon]` [Detay / Sil / PDF]
  - **Koşul:** (Örn: `pdf_path` doluysa aktif)
  - **Davranış:** ...

---

## 🛠 Teknik Notlar & Gereksinimler

### 🔌 API Entegrasyonu
- `GET /api/v1/...` -> Listeleme
- `POST /api/v1/...` -> İşlem tetikleme

### 💾 Veritabanı & Mapping
- **Tablo:** `tablo_adi`(Örnektir)
- **Mapping:** `taxpayer_id` -> Frontend'de isim olarak gösterilecek.(Örnektir)

### ⚙️ State & Logic
- İşlem başladığında `loading` state gösterilmeli.(Örnektir)
- Modal onayı alınmadan işlem yapılmamalı.(Örnektir)

---

## ✅ Kabul Kriterleri (Acceptance Criteria)
- [ ] ............
- [ ] ............
- [ ] ............
- [ ] ............