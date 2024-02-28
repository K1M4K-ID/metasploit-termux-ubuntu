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
- **update & upgrade**: Langkah berikut nya setelah login ke dalam ubuntu, update & upgrade terlebih dahulu.
  ```
  apt update && apt upgrade -y
  ```
- **install metasploit**: Langkah berikut nya install metasploit, tunggu sampai 15-30 menit tergantung speed internet.
  ```
  curl https://raw.githubusercontent.com/rapid7/metasploit-omnibus/master/config/templates/metasploit-framework-wrappers/msfupdate.erb > msfinstall && \
  chmod 755 msfinstall && \
  ./msfinstall
  ```
- **install zipalign**: Langkah berikut nya install zipalign
  ```
  apt-get --purge remove zipalign #jika sudah pernah install zipalign kalau belum lewati bagian ini

  git clone https://github.com/K1M4K-ID/fix-zipalign;cd fix-zipalign;chmod +x fix-zipalign.sh;bash fix-zipalign.sh
  ```

  ## selesai
  selamat bersenang senang, installer by K1M4K-ID
  
