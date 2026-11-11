# Simulasi Tanggap Darurat Gempa UPTBKU 2026

Tampilan TV simulasi Tabletop Exercise (TTX) BCP untuk syuting di ruang Raflesia,
PT PLN (Persero) UPT Bengkulu – UIP3B Sumatera.

## Skenario

Skrip Final Blocking Simulasi Tabletop Exercise (TTX) BCP
(SKP/TTX.BCP/UPT-BKL/2026.002, pelaksanaan 07 November 2026):

- Gempa bumi tektonik **7,3 M**, 08.00 WIB, episentrum 45 km barat daya Kota Bengkulu,
  guncangan 45 detik, Level Risiko 21 (Katastropik).
- SUTT 150 kV Pekalongan–Sukamerindu–Pulau Baai–Manna trip bersamaan
  → blackout total Provinsi Bengkulu, telemetri SCADA drop.
- **103 personel 100% selamat**, zero accident.
- GI Tes & GI Pulau Baai hilang kontak; bushing Trafo Daya 1 60 MVA GI Sukamerindu
  retak + kebocoran minyak; longsor memutus SUTT Pekalongan–Tes dan menutup akses
  Lahat–Manna (Bukit Sumbul); kantor UPT retak → Alternate Site GI Sukamerindu.
- F1 pulih **1 jam 50 menit** via black-start PLTA Tes (09.50 WIB, RTO 2 jam tercapai);
  F2 pulih **100% hari ke-5** (RTO 1 minggu tercapai); hari ke-15 re-entry kantor,
  BCP resmi ditutup. MBCO 8.135 MW; beban prioritas: RS M. Yunus, Bandara Fatmawati,
  Kantor Gubernur.

## Isi tampilan (`index.html`)

Satu file HTML mandiri (16:9, full-screen TV):

- 6 fase yang bisa diklik — Normal → Gempa & Blackout Total → BCP Direkomendasikan →
  Black-Start PLTA Tes 09.50 & BCP Aktif → Pemulihan 100% hari ke-5 → BCP Ditutup hari ke-15.
  Tiap fase mengubah banner, jam simulasi, KPI beban/frekuensi/GI/SCADA, status GI,
  panel keselamatan, grafik pemulihan, log dispatcher, dan ticker.
- Diagram single-line 150 kV, grafik pemulihan beban + status RTO F1/F2,
  CCTV 2×2 (GI Sukamerindu, GI Tes, Kantor UPT/Raflesia, SUTT 150 kV).
- Mode Putar Otomatis (±10 detik/fase), tombol Layar Penuh TV, navigasi keyboard ←/→.

## Menampilkan di TV

Buka URL deployment Vercel repo ini di browser TV, lalu tekan Layar Penuh.
Semua data di atas adalah **SIMULASI** sesuai naskah TTX BCP — bukan kondisi nyata.

## Aset UPT Bengkulu (konteks)

15 Gardu Induk, 33 sirkit, 34 trafo 2.475 MVA, 2.424 tower / 1.582,72 kms,
2 ULTG (Pekalongan & Lahat).
