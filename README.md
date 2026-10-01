# ProStrike by ProKuiz 🎯

Game tembak pasukan 3D gaya Counter-Strike — **17 senjata (semua percuma)**, **10 kawasan = 10 level**, **Misi Bot**, **Lawan Online 1v1 / 2v2 / 3v3** (dengan kawan bot), ranking & mod **Latihan**.
Konsep sama macam ProFighter/ProChess: APK buka versi live di GitHub Pages → **kemas kini automatik tanpa download APK baru**.

## Pasukan
🐯 **HARIMAU** (oren) lawan 🦅 **HELANG** (biru). Hapuskan semua musuh untuk menang pusingan — **pasukan pertama menang 4 pusingan** menang perlawanan.
Setiap pusingan: 4 saat bersedia → 1:45 bertempur. Mati = tonton rakan sepasukan (boleh laju ⏩ x2/x3 dalam misi bot).

## Senjata (pilih mana-mana di awal pusingan — butang 🛒 SENJATA)
| Jenis | Senjata |
|---|---|
| Pistol | P-9 · S-45 Senyap (musuh susah dengar) · D-50 Helang · R-8 Revolver |
| SMG | MP-9 · P-50 (50 peluru) · U-45 |
| Shotgun | Pam-12 · Auto-12 |
| Raifal | AK-47 · M4A1 · G-3X · SG-8 Skop 🎯 |
| Sniper | HAWK .338 (2 tahap zum) · SCOUT · AUTO-SNIPER |
| LMG | LMG-100 (100 peluru) |
| Lain | 🔪 Kerambit (tikam dari belakang = mati) · 💣 Bom tangan · 💨 Bom asap |

**Peluru tanpa had** — tak perlu isi semula (butang ISI dibuang). Tembakan kepala = kerosakan x4 (raifal). Tunduk & berdiri diam = lebih tepat. Berlari/melompat = kurang tepat. Rekoil naik bila tembak lama.

## 10 Kawasan (Level)
1 Kampung · 2 Gudang · 3 Pelabuhan · 4 Padang Pasir · 5 Hutan · 6 Bandar · 7 Kilang · 8 Pangkalan Salji · 9 Stesen MRT · 10 Istana Malam
- Menang level untuk buka kawasan seterusnya. Bot makin pandai setiap level (reaksi, ketepatan, tembakan kepala, gerak tepi, bom tangan).
- Bintang: ★ menang · ★★ menang beza 2 · ★★★ menang beza 3+
- Saiz pasukan boleh pilih: 3v3 · 4v4 · 5v5 (anda + kawan bot).
- Setiap peta dijana simetri (separuh atas diputar 180°) supaya adil untuk dua pasukan.

## Online
- **Mod:** 1v1 · 2v2 · 3v3. **Kawan bot** (suis): pasukan dilengkapkan bot hingga 5 orang. 1v1 = bot ON secara lalai, 2v2/3v3 = manusia sahaja (boleh tukar).
- **Buat Bilik** — dapat kod 5 huruf, kawan masuk guna kod. Hos pilih peta, pemain boleh **Tukar Pasukan**, hos tekan **Mula Sekarang** (tempat kosong diisi bot).
- **Ajak** pemain dari senarai online → mereka masuk ke bilik anda.
- Rangkaian: hos (pencipta bilik) jalankan permainan & bot; tetamu sambung terus **P2P (WebRTC)**. Jika P2P tak dapat, automatik guna **Relay Firestore**. Label ⚡ P2P / ☁️ Relay dipapar di kiri atas.
- Pemain keluar → bot ambil alih watak dia. Hos keluar → perlawanan tamat.
- Rating ELO + pangkat 🥉 Gangsa → 🥈 Perak (1100) → 🥇 Emas (1250) → 💠 Platinum (1400) → 💎 Berlian (1600) → 👑 Legenda (1800).

## Kawalan
**Telefon:** joystick kiri (gerak) · seret skrin kanan (pandang) · 🔫 TEMBAK (boleh seret untuk bidik sambil tembak) · 🎯 SKOP · 🔄 ISI · ⤴️ LOMPAT · ⬇️ TUNDUK · 💣 · 💨 · ketik ikon senjata di bawah untuk tukar.
**Tetapan:** kepekaan pandangan, **tembak automatik** (tembak sendiri bila crosshair pada musuh — sesuai budak/pemula), **bantuan bidik**, butang tembak kiri, kualiti grafik, butang besar.
**PC / laptop:** Tetapan → hidupkan **Main guna PC** (lalai ON bila dibuka di komputer). Semua butang skrin sentuh disembunyikan; kawal guna papan kekunci + tetikus (tetikus hanya dikunci bila anda klik skrin permainan; tekan **Esc** untuk lepaskan tetikus — game berehat. Bila anda klik tetingkap lain / alt-tab, game berehat & berhenti melukis supaya komputer tak lag).
- **Susunan kekunci siap:** ⌨️ WASD · ⬆️ Anak Panah (gerak guna anak panah, pandang guna W/A/S/D, tembak X, skop Z) · 🔢 Nombor (gerak 8/4/5/6 pada numpad atau baris nombor, tembak Enter).
- **Saiz paparan:** dalam mod PC semua ikon, butang, peta mini & HUD dibesarkan ikut saiz skrin. Pilih S / M / L / **MAX** (lalai MAX = paling besar yang muat).
- **Ubah sendiri:** tekan butang kekunci dalam senarai → tekan kekunci baru (Backspace = kosongkan, Esc = batal). Kekunci yang sama dibuang dari tindakan lain secara automatik.
- Ada kekunci **pandang kiri/kanan/atas/bawah** — sesuai untuk laptop guna touchpad. **Kepekaan tetikus** boleh dilaras berasingan.

## Grafik
Enjin **WebGL 3D sendiri** dalam `index.html` (tiada library luar — ringan & boleh main misi bot offline): peta bertekstur prosedur (bata, peti, kontena, jubin, tingkap bercahaya waktu malam), bayang lembut, kabus, langit, pokok, kereta, kren, askar 3D beranimasi, senjata tangan dengan rekoil & animasi isi peluru, kesan peluru, asap & letupan.
Phone lambat: **Tetapan → Kualiti grafik → Rendah**.

## Setup (sekali sahaja)
1. **Repo GitHub `alemmaxx/ProStrike`** (Public) → upload semua fail ini ke branch `main` (termasuk `.github`, `.nojekyll`).
2. **GitHub Pages**: Settings → Pages → *Deploy from a branch* → `main` / `(root)` → Save.
   App hidup di `https://alemmaxx.github.io/ProStrike/`
3. **Secret** `KEYSTORE_BASE64` (Settings → Secrets and variables → Actions) — isi sama macam ProFighter/ProChess.
4. **Firebase** (projek `prokuiz-aplikasi-b518a`, sama dengan ProFighter):
   - Authentication → Anonymous → sepatutnya dah **Enable**
   - **Firestore Database → Rules** → ganti dengan isi fail `firestore.rules` → **Publish**
     (fail ini = rules ProSudoku + ProChess + ProFighter sedia ada + blok ProStrike baru; app lain tak terjejas)
5. Tab **Actions** → build siap → **Releases** → muat turun `ProStrike.apk` → pasang.

## Kemas kini app selepas ini
1. Edit `index.html` → **naikkan `APP_VERSION`** (cth `'1.0.0'` → `'1.0.1'`).
2. Push ke `main`. App pengguna tunjuk bar **Kemas Kini** berkelip → tekan → siap.
   APK baru hanya perlu kalau tukar `capacitor.config.json` / ikon / plugin.

## Password admin padam ranking
Sama dengan app lain (`adminPassword()` dalam `firestore.rules`). ProStrike guna dokumen `config/strike`, jadi padam ranking ProStrike tak kacau app lain.

## Struktur
| Fail | Fungsi |
|---|---|
| `index.html` | Seluruh game (enjin 3D, peta, senjata, bot, online) |
| `sw.js`, `manifest.webmanifest`, `icons/` | PWA / iPhone / cache offline |
| `offline.html` | Skrin "Tiada Internet" dalam APK |
| `capacitor.config.json` | APK buka `https://alemmaxx.github.io/ProStrike/` |
| `firestore.rules` | Rules gabungan ProSudoku + ProChess + ProFighter + ProStrike |
| `.github/workflows/build-apk.yml` | Build APK (landscape, skrin penuh) + release |
| `assets/` | Ikon & splash untuk APK |
