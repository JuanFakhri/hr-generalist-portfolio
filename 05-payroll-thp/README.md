# 05 — Perhitungan THP & Administrasi Kompensasi
### Studi Kasus Payroll Karyawan · HR Bootcamp Basic Mission 4 · Skor 80

[![Project](https://img.shields.io/badge/Project-Basic_Mission_4-2D9CDB?style=flat-square)]()
[![Score](https://img.shields.io/badge/Skor-80%2F100-27AE60?style=flat-square)]()
[![Tools](https://img.shields.io/badge/Tools-Google_Sheets_%7C_Regulasi_BPJS-F4A261?style=flat-square)]()

---

## 📌 Problem Statement

Perusahaan memiliki **5 karyawan** dengan status kepesertaan BPJS yang berbeda-beda (sebagian ditanggung perusahaan, sebagian ditanggung sendiri). Diperlukan perhitungan **Take Home Pay (THP) yang akurat dan sesuai regulasi** — termasuk pemotongan BPJS per individu, PPh 21 dasar, dan penyusunan slip gaji terstandarisasi.

---

## 🎯 Tujuan & Output

| Tujuan | Output yang Dihasilkan |
|--------|----------------------|
| Hitung THP bersih tiap karyawan | Spreadsheet THP 5 karyawan |
| Terapkan komponen BPJS per regulasi | Breakdown iuran BPJS per karyawan |
| Susun slip gaji terstandarisasi | Format slip gaji siap cetak |

---

## 📊 Komponen Perhitungan THP

### Struktur Gaji
```
PENGHASILAN KOTOR
├── Gaji Pokok
├── Tunjangan Jabatan
├── Tunjangan Transport
└── Tunjangan Makan
                    = TOTAL PENGHASILAN BRUTO

POTONGAN
├── BPJS Ketenagakerjaan — Iuran Karyawan
│   ├── JHT  (Jaminan Hari Tua)        → 2%  dari gaji pokok
│   └── JP   (Jaminan Pensiun)         → 1%  dari gaji pokok
├── BPJS Kesehatan                     → 1%  dari gaji pokok (maks. Rp 12jt)
└── PPh 21 (Pajak Penghasilan)         → sesuai tarif progresif PTKP
                    = TOTAL POTONGAN

TAKE HOME PAY (THP) = Penghasilan Bruto − Total Potongan
```

### Iuran BPJS — Ditanggung Perusahaan
| Komponen | Tarif | Ditanggung |
|----------|-------|-----------|
| JHT (Jaminan Hari Tua) | 3.7% | Perusahaan |
| JP (Jaminan Pensiun) | 2% | Perusahaan |
| JKK (Jaminan Kecelakaan Kerja) | 0.24% | Perusahaan |
| JKM (Jaminan Kematian) | 0.30% | Perusahaan |
| BPJS Kesehatan | 4% | Perusahaan |

### Iuran BPJS — Ditanggung Karyawan
| Komponen | Tarif | Keterangan |
|----------|-------|-----------|
| JHT | 2% | Dipotong dari gaji |
| JP | 1% | Dipotong dari gaji |
| BPJS Kesehatan | 1% | Maks. dari gaji Rp 12.000.000 |

---

## 📋 Simulasi THP (Contoh 1 Karyawan)

```
Nama              : Karyawan A (Status: BPJS ditanggung perusahaan)
Gaji Pokok        : Rp 5.000.000
Tunjangan Jabatan : Rp 500.000
Tunjangan Transport: Rp 300.000
Tunjangan Makan   : Rp 200.000
─────────────────────────────────
Penghasilan Bruto : Rp 6.000.000

Potongan Karyawan:
  JHT  (2%)       : Rp   100.000
  JP   (1%)       : Rp    50.000
  BPJS Kes (1%)   : Rp    50.000
  PPh 21          : Rp         0  (di bawah PTKP)
─────────────────────────────────
Total Potongan    : Rp   200.000

TAKE HOME PAY     : Rp 5.800.000
```

---

## 📁 Dokumen dalam Folder Ini

| File | Keterangan |
|------|-----------|
| `THP-Calculation-Guide.md` | Panduan lengkap perhitungan THP, formula, dan simulasi 5 karyawan |

> 📌 *File spreadsheet asli (Google Sheets) tersedia untuk review — hubungi via email.*

---

## 📚 Referensi Regulasi

- PP No. 45 Tahun 2015 — Iuran Jaminan Pensiun
- PP No. 44 Tahun 2015 — Jaminan Kecelakaan Kerja & Kematian
- Perpres No. 82 Tahun 2018 — BPJS Kesehatan
- UU No. 36 Tahun 2008 — Pajak Penghasilan (PPh 21)

---

## 🔗 Keterkaitan Project

- Manpower Planning & budget SDM → lihat [`03-manpower-planning/`](../03-manpower-planning/)
