mkdir : membuat folder baru melalui terminal

-p : kepanjangan dari --parents, digunakna di mkdir. ada dua fungsi memuat jalur bertingkat(folder belom ada sistem otomatis membuatkannya) dan mode aman (folder sudah ada, tidak memunculkan error dan folder lama aman tampa timpa). 

mkdir -p : co1 (mkdir -p note linux python sql projects), hasilnya 5 folder terpisah sejajar dalam direktori aktif saat ini. co2 (mkdir -p data/raw/transaksi/2026), hasilnya 4 lapis folder bersarang berurutan data --> raw dst.

touch : perintah untuk membuat file kosong baru 

.gitkeep : penanda agar file kosong tetap terdeteksi oleh git

git pull: mengunduh pembaharuan kode terbaru dari github ke laptop (memastikan scrip kode selalu singkron dengan pekerjakan rekan tim lainya) git pull origin main

git checkout -b : membuat cabang baru (branch) sekaligus pindah. kegunaan perubahan kode atau perbaikan bug agar tidak merusak pipeline utama (main) yg sedang berjalan. git checkout -b fix/pembayaran

git status : mengecek daftar file yg baru di buat, diubah, atau belom di simpan. memastikan tidak ada data rahasia yg tidak sengaja ikut terbawa sebelum git push (selalau cek git status sebelum menjalankan add).

git add dan git commit : memilih file (add) dan mengunci riwayat perubahan (commit) berserta catatan. meciptakan titik simpan (checkpoin) yg jelas sehinga kode mudah di lacak atau di kembalikan jika suatu saat terjadi error. git add . / git add extract.py  /  git commit -m "fix/pembayaran"

git push : mengunggah seluruh commit dari laptop ke server github. mencadangkan kode ke cloud dan mengirin ke rekan tim untuk di periksa sebelum di gabung kesistem utama. git push -u origin feat/etl-penjualan

.gitignore : daftar aturan file/folder yg wajib di abaikan oleh git. mencagah kecbocoran ps databse (.env), dan mencagah file data set raksasa membebani repo gihub. 


