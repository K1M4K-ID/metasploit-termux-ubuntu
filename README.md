# metasploit-termux-ubuntu
How To Install Metasploit Termux Ubuntu

### Langkah - Langkah:
- **Update & Upgrade**: Langkah pertama update dan upgrade termux terlebih dahulu.
  ```
  apt update && apt upgrade -y
  ```
- **install distro ubuntu**: Langkah berikut nya install proot dan proot-distro untuk menginstall ubuntu pada termux, tidak memerlukan root akses.
  ```
  apt install proot proot-distro;proot-distro install ubuntu
  ```
- **membuat script login ubuntu**: Langkah berikut nya, setelah menginstall ubuntu pada termux, kita bisa login ke ubuntu dengan perintah proot-distro login ubuntu atau kita bisa membuat script yang sederhana untuk login ke ubuntu silahkan coppy paste.
  ```
  echo "proot-distro login ubuntu" > $PREFIX/bin/ubuntu
  ```
  lalu ketik perintah ubuntu, untuk login ke ubuntu
