# ThirdWeb API Configuration Guide

## Cara Mendapatkan Client ID

1. Buka [ThirdWeb Dashboard](https://thirdweb.com/dashboard)
2. Login ke akun anda (Registrasi dahulu jika belum ada)
3. Koneksikan wallet yang sama seperti di Rewardable ke akun ThirdWeb
4. Buat Project baru dan klik Project yang sudah dibuat
5. Klik tab "Settings" (pengaturan)
6. Pilih "ClientID"
7. Salin Client ID yang sudah ada
8. Simpan Client ID kedalam file .env

## Setup File Environment (.env)

Buat file `.env` di folder utama project dan konfigurasi variabel berikut:

```env
PRIVATE_KEY=         # Private key dari wallet anda
CLIENT_ID=           # Client ID dari dashboard ThirdWeb
CONTRACT_ADDRESS=    # Alamat smart contract yang sudah di-deploy
IDENTITY_ADDRESS=    # Alamat kontrak identity (jika digunakan)
WITHDRAWAL_AMOUNT=   # Jumlah untuk transaksi penarikan
TX_DATA=            # Data transaksi jika diperlukan
```

### Detail Konfigurasi

- `PRIVATE_KEY`: Private key dari wallet (jangan pernah dibagikan)
- `CLIENT_ID`: Client ID API dari dashboard ThirdWeb
- `CONTRACT_ADDRESS`: Alamat kontrak pintar yang sudah di-deploy
- `IDENTITY_ADDRESS`: Diperlukan jika menggunakan verifikasi identitas
- `WITHDRAWAL_AMOUNT`: Jumlah penarikan dalam Wei
- `TX_DATA`: Data transaksi dalam format hexadecimal (Dari Explorer)

### Running Script

```bash
# Clone repository
git clone https://github.com/Langga40/Rewardable.git

# Install dependencies
npm install

# Setup environment variables
setup file .env

# Run the application
node index.js
```

### Donate
You can donate me if you want : `0x04caeb08D47Df2E039a3B3aDEDd49ABcb7E8FA0e`
