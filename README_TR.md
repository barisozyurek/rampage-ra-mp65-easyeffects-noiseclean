# 🎤 Rampage RA-MP65 — EasyEffects Gürültü Temizleme Preseti

> **Ana dil: İngilizce**  
> English version: [README.md](README.md)

Bu depo, **Rampage RA-MP65 X-FUSE USB mikrofon** için özel olarak ayarlanmış
bir **EasyEffects gürültü temizleme preset’i** içerir.

Bu preset şu sorunları gerçek zamanlı olarak giderir:

- Elektronik cızırtı
- Sabit “bip” sesleri
- USB kaynaklı parazit
- Arka plan uğultusu

Basit noise gate çözümlerinden farklı olarak bu preset,  
**RNNoise ve DeepFilterNet adlı iki sinir ağı (neural network) tabanlı gürültü bastırma motorunu** kullanır.  
Bu motorlar, sesi ve gürültüyü öğrenilmiş modellerle ayırt ederek yalnızca
istenmeyen sesleri bastırır ve sesi doğal bırakır.

Şunlar için idealdir:

- 🎮 Oyun & Discord
- 🎙 Sesli sohbet
- 📹 Yayın & kayıt
- 💻 Online toplantılar

---

## 📁 Dosyalar

- `rampage-ra-mp65-clean.json` — EasyEffects preset dosyası

---

## 🧰 Gereksinimler

- Linux (PipeWire)
- EasyEffects 7+
- DeepFilterNet eklentisi

### DeepFilterNet Kurulumu (Arch / CachyOS)

```bash
paru -S libdf-git libdeep_filter_ladspa-git
```

Diğer dağıtımlar için paket yöneticinizde:
`deepfilter`, `libdeep_filter`, `ladspa-deepfilter` arayın.

---

## ⚙ Kurulum

1. EasyEffects’i aç
2. **Presets → Import**
3. `rampage-ra-mp65-clean.json` dosyasını seç
4. Preseti uygula
5. Mikrofon girişinin doğru seçili olduğundan emin ol

---

## 🔊 Efekt Zinciri

| Efekt | Görevi |
|--------|--------|
| **RNNoise** | Sürekli gürültüyü temizler |
| **DeepFilterNet** | Sinir ağı tabanlı ses ayıklama |
| **Gate** | Sessizlikte mikrofonu kapatır |

---

## 🛠 İpuçları

- Mikrofon seviyesini **%70–85** aralığında tut
- USB hub kullanma
- Pop filter kullan
- Ses kesiliyorsa Gate threshold’u biraz düşür
