# Panduan Lengkap Perhitungan THP & Administrasi BPJS
### Studi Kasus: 5 Karyawan dengan Status BPJS Berbeda

---

## 🎯 Tujuan Dokumen

Dokumen ini merupakan panduan praktis perhitungan **Take Home Pay (THP)** yang sesuai regulasi ketenagakerjaan Indonesia — mencakup komponen gaji, iuran BPJS Ketenagakerjaan, BPJS Kesehatan, dan PPh 21 dasar.

---

## 📋 Data 5 Karyawan (Simulasi)

| No | Nama | Jabatan | Gaji Pokok | Status BPJS |
|----|------|---------|-----------|-------------|
| 1 | Karyawan A | Supervisor | Rp 5.000.000 | ✅ Ditanggung perusahaan |
| 2 | Karyawan B | Staff Admin | Rp 3.500.000 | ✅ Ditanggung perusahaan |
| 3 | Karyawan C | Operator | Rp 3.000.000 | ✅ Ditanggung perusahaan |
| 4 | Karyawan D | Kasir | Rp 3.200.000 | ❌ Tidak didaftarkan BPJS |
| 5 | Karyawan E | Helper | Rp 2.800.000 | ⚠️ Hanya BPJS Kesehatan |

---

## 🔢 Formula Perhitungan

### Step 1 — Hitung Penghasilan Bruto
```
Penghasilan Bruto = Gaji Pokok + Tunjangan Jabatan + Tunjangan Transport + Tunjangan Makan
```

### Step 2 — Hitung Iuran BPJS Karyawan
```
JHT Karyawan     = 2%  × Gaji Pokok
JP Karyawan      = 1%  × Gaji Pokok
BPJS Kes Karyawan= 1%  × Gaji Pokok  (maks. dasar perhitungan Rp 12.000.000)

Total Iuran BPJS = JHT + JP + BPJS Kes
```

### Step 3 — Hitung PPh 21 (Bulanan)
```
Penghasilan Neto/Tahun = (Bruto - Iuran BPJS) × 12
PTKP (TK/0)            = Rp 54.000.000/tahun
PKP                    = Penghasilan Neto - PTKP

Tarif Progresif:
  PKP ≤ Rp 50jt       → 5%
  Rp 50jt – Rp 250jt  → 15%
  Rp 250jt – Rp 500jt → 25%

PPh 21 Bulanan = PKP × Tarif ÷ 12
```

### Step 4 — Hitung THP
```
THP = Penghasilan Bruto − Total Iuran BPJS Karyawan − PPh 21 Bulanan
```

---

## 📊 Tabel THP Lengkap 5 Karyawan

| | A (Supervisor) | B (Admin) | C (Operator) | D (Kasir) | E (Helper) |
|--|---------------|-----------|--------------|-----------|------------|
| Gaji Pokok | 5.000.000 | 3.500.000 | 3.000.000 | 3.200.000 | 2.800.000 |
| Tunjangan Total | 1.000.000 | 700.000 | 600.000 | 600.000 | 500.000 |
| **Bruto** | **6.000.000** | **4.200.000** | **3.600.000** | **3.800.000** | **3.300.000** |
| JHT (2%) | 100.000 | 70.000 | 60.000 | — | — |
| JP (1%) | 50.000 | 35.000 | 30.000 | — | — |
| BPJS Kes (1%) | 50.000 | 35.000 | 30.000 | — | 28.000 |
| PPh 21 | — | — | — | — | — |
| **Total Potongan** | **200.000** | **140.000** | **120.000** | **0** | **28.000** |
| **THP** | **5.800.000** | **4.060.000** | **3.480.000** | **3.800.000** | **3.272.000** |

> *Semua karyawan di bawah nilai PKP — PPh 21 = Rp 0*

---

## 💰 Rekap Beban Perusahaan (Iuran Employer)

| Komponen | Tarif | Karyawan A | Karyawan B | Karyawan C |
|----------|-------|-----------|-----------|-----------|
| JHT (3.7%) | 3.7% | 185.000 | 129.500 | 111.000 |
| JP (2%) | 2% | 100.000 | 70.000 | 60.000 |
| JKK (0.24%) | 0.24% | 12.000 | 8.400 | 7.200 |
| JKM (0.30%) | 0.30% | 15.000 | 10.500 | 9.000 |
| BPJS Kes (4%) | 4% | 200.000 | 140.000 | 120.000 |
| **Total/karyawan** | | **512.000** | **358.400** | **307.200** |

---

## 📎 Catatan Penting

1. **BPJS wajib** didaftarkan untuk seluruh karyawan tetap (PKWTT) — perusahaan yang tidak mendaftarkan dapat dikenai sanksi administratif
2. **Batas atas gaji** untuk perhitungan JP: Rp 9.559.600/bulan (UMP 2025)
3. **BPJS Kesehatan**: batas atas dasar perhitungan iuran = Rp 12.000.000/bulan
4. **PPh 21** dihitung setahun, dibagi 12 — perlu disesuaikan jika ada penghasilan tidak teratur (bonus, THR)
