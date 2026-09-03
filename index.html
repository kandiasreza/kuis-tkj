<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Kuis - Alat-Alat TKJ</title>
<style>
  body {
    font-family: 'Segoe UI', Arial, sans-serif;
    background: #f4f6f8;
    color: #222;
    max-width: 850px;
    margin: 0 auto;
    padding: 30px 20px 60px;
    line-height: 1.6;
  }
  header {
    text-align: center;
    border-bottom: 3px solid #1a5276;
    padding-bottom: 15px;
    margin-bottom: 25px;
  }
  header h1 { color: #1a5276; margin-bottom: 5px; }
  header p { margin: 3px 0; color: #555; }

  .identitas {
    background: #eaf2f8;
    border: 1px solid #aed6f1;
    border-radius: 8px;
    padding: 12px 18px;
    margin-bottom: 20px;
  }
  .identitas input {
    border: none;
    border-bottom: 1px solid #aed6f1;
    background: transparent;
    font-size: 1em;
    padding: 2px 4px;
    width: 250px;
  }
  .identitas p.hint { color:#b9770e; font-size:0.9em; margin-top:8px; }

  #btn-start {
    display: block;
    margin: 0 auto 25px;
  }

  #progress-bar-wrap {
    background: #dcdcdc;
    border-radius: 6px;
    height: 10px;
    margin-bottom: 20px;
    overflow: hidden;
  }
  #progress-bar {
    background: #1a5276;
    height: 100%;
    width: 0%;
    transition: width .3s;
  }

  .soal {
    background: #fff;
    border: 1px solid #dcdcdc;
    border-radius: 8px;
    padding: 15px 20px;
    margin-bottom: 16px;
  }
  .soal p.pertanyaan {
    font-weight: 600;
    margin-bottom: 10px;
  }
  .pilihan {
    list-style: none;
    padding-left: 0;
    margin: 0;
  }
  .pilihan li {
    padding: 8px 10px;
    margin-bottom: 6px;
    border-radius: 6px;
    cursor: pointer;
    border: 1px solid #e0e0e0;
    transition: background .15s;
  }
  .pilihan li:hover { background: #f0f6fb; }
  .pilihan li.selected {
    background: #d6eaf8;
    border-color: #1a5276;
  }
  .pilihan li.correct {
    background: #d5f5e3;
    border-color: #27ae60;
  }
  .pilihan li.incorrect {
    background: #fadbd8;
    border-color: #e74c3c;
  }
  .pilihan li span.label {
    display: inline-block;
    width: 22px;
    font-weight: bold;
    color: #1a5276;
  }
  .pilihan li.locked { cursor: default; }

  #btn-row {
    text-align: center;
    margin: 30px 0;
  }
  button {
    background: #1a5276;
    color: #fff;
    border: none;
    padding: 12px 28px;
    font-size: 1em;
    border-radius: 6px;
    cursor: pointer;
  }
  button:hover { background: #154360; }
  button:disabled { background: #aaa; cursor: not-allowed; }
  button.secondary { background: #b9770e; }
  button.secondary:hover { background: #935f0b; }

  #hasil {
    display: none;
    text-align: center;
    background: #fdf2e9;
    border: 1px solid #f5b041;
    border-radius: 10px;
    padding: 25px;
    margin-top: 20px;
  }
  #hasil h2 { color: #b9770e; margin-top: 0; }
  #skor {
    font-size: 2.2em;
    font-weight: bold;
    color: #1a5276;
  }
  #hasil-buttons button { margin: 6px; }

  #riwayat {
    margin-top: 30px;
    background: #fff;
    border: 1px solid #dcdcdc;
    border-radius: 8px;
    padding: 15px 20px;
  }
  #riwayat h3 { color: #1a5276; margin-top: 0; }
  table { width: 100%; border-collapse: collapse; font-size: 0.95em; }
  table th, table td {
    border-bottom: 1px solid #e0e0e0;
    padding: 6px 8px;
    text-align: left;
  }
  table th { color: #1a5276; }

  #quiz-area.hidden, #btn-row.hidden, #start-area.hidden { display: none; }

  footer {
    text-align: center;
    margin-top: 40px;
    color: #888;
    font-size: 0.9em;
  }
</style>
</head>
<body>

<header>
  <h1>KUIS ALAT-ALAT TKJ</h1>
  <p>Alat-Alat Teknik Komputer dan Jaringan (TKJ)</p>
</header>

<div id="start-area">
  <div class="identitas">
    <p>Nama&nbsp;: <input type="text" id="nama" placeholder="Tulis nama..."></p>
    <p>Kelas&nbsp;: <input type="text" id="kelas" placeholder="Tulis kelas..."></p>
    <p>Jumlah Soal&nbsp;: 35 (Pilihan Ganda)</p>
    <p class="hint">Urutan soal dan pilihan jawaban akan diacak secara otomatis setiap kali kuis dimulai.</p>
  </div>
  <button id="btn-start">Mulai Kuis</button>
</div>

<div id="progress-bar-wrap" style="display:none;"><div id="progress-bar"></div></div>
<p id="progress-text" style="text-align:center; color:#555;"></p>

<div id="quiz-area" class="hidden"></div>

<div id="btn-row" class="hidden">
  <button id="btn-next" disabled>Jawaban Selanjutnya</button>
</div>

<div id="hasil">
  <h2>Hasil Kuis</h2>
  <p>Nama: <span id="hasil-nama"></span> | Kelas: <span id="hasil-kelas"></span></p>
  <p id="skor"></p>
  <p id="skor-detail"></p>
  <div id="hasil-buttons">
    <button id="btn-restart" class="secondary">Ulangi Kuis</button>
    <button id="btn-download">Unduh Hasil (CSV)</button>
  </div>
</div>

<div id="riwayat">
  <h3>Riwayat Nilai Tersimpan (di perangkat ini)</h3>
  <table id="tabel-riwayat">
    <thead><tr><th>Nama</th><th>Kelas</th><th>Skor</th><th>Nilai</th><th>Waktu</th></tr></thead>
    <tbody></tbody>
  </table>
  <p id="riwayat-kosong" style="color:#888;">Belum ada riwayat.</p>
  <button id="btn-clear-riwayat" class="secondary" style="margin-top:10px;">Hapus Riwayat</button>
</div>

<footer>
  <p>Kuis Interaktif - Materi Alat-Alat TKJ</p>
</footer>

<script>
// ===== Data soal asli (urutan tetap A/B/C/D sesuai jawaban benar aslinya) =====
const soalAsli = [
{q:"Alat yang digunakan untuk memasang konektor RJ-45 pada kabel UTP disebut...", opts:["LAN Tester","Crimping Tool","Cable Stripper","Obeng"], ans:1},
{q:"Fungsi utama LAN Tester adalah...", opts:["Memotong kabel fiber optik","Menguji koneksi/urutan kabel UTP","Mengukur tegangan listrik","Menyambung kabel coaxial"], ans:1},
{q:"Alat untuk mengupas kulit luar kabel UTP tanpa merusak inti kabel disebut...", opts:["Punch Down Tool","Cable Stripper","Tang Ampere","Multimeter"], ans:1},
{q:"Alat yang digunakan untuk menekan kabel ke dalam modul keystone atau patch panel disebut...", opts:["Crimping Tool","Punch Down Tool (LSA Tool)","Cutter","Obeng Plus"], ans:1},
{q:"Perangkat yang berfungsi menghubungkan beberapa komputer dalam satu jaringan LAN dan meneruskan data berdasarkan alamat MAC adalah...", opts:["Router","Switch","Modem","Access Point"], ans:1},
{q:"Perangkat yang berfungsi menghubungkan dua jaringan berbeda dan mengatur jalur data (routing) adalah...", opts:["Hub","Router","Repeater","Bridge"], ans:1},
{q:"Alat yang mengubah sinyal digital menjadi sinyal analog dan sebaliknya untuk koneksi internet disebut...", opts:["Switch","Modem","NIC","Access Point"], ans:1},
{q:"Perangkat yang memancarkan sinyal WiFi sehingga perangkat lain dapat terhubung secara nirkabel disebut...", opts:["Access Point","Router kabel","Hub","Bridge"], ans:0},
{q:"Kartu jaringan yang dipasang pada komputer agar dapat terhubung ke jaringan disebut...", opts:["NIC (Network Interface Card)","VGA Card","Sound Card","Patch Panel"], ans:0},
{q:"Alat yang berfungsi memperkuat sinyal jaringan agar dapat menjangkau jarak yang lebih jauh disebut...", opts:["Repeater","Switch","Konektor","Patch Cord"], ans:0},
{q:"Konektor yang digunakan pada ujung kabel UTP untuk jaringan Ethernet adalah...", opts:["RJ-11","RJ-45","BNC","USB Type-C"], ans:1},
{q:"Konektor RJ-11 umumnya digunakan pada perangkat...", opts:["Kabel LAN","Kabel telepon","Kabel fiber optik","Kabel coaxial"], ans:1},
{q:"Alat ukur yang digunakan untuk mengukur tegangan, arus, dan resistansi listrik disebut...", opts:["Multimeter","LAN Tester","OTDR","Cable Tester"], ans:0},
{q:"Alat yang digunakan untuk memotong dan mengupas kabel fiber optik dengan presisi disebut...", opts:["Fiber Cleaver","Crimping Tool","Tang Kombinasi","Cable Stripper"], ans:0},
{q:"Alat untuk menyambung dua ujung kabel fiber optik menggunakan proses pelelehan (fusion) disebut...", opts:["Fusion Splicer","Fiber Cleaver","OTDR","Media Converter"], ans:0},
{q:"OTDR (Optical Time Domain Reflectometer) digunakan untuk...", opts:["Mengukur kecepatan internet","Mendeteksi titik putus atau redaman pada kabel fiber optik","Memotong kabel UTP","Mengatur konfigurasi router"], ans:1},
{q:"Perangkat yang berfungsi mengubah sinyal optik menjadi sinyal listrik atau sebaliknya disebut...", opts:["Media Converter","Splicer","Patch Panel","Switch Manageable"], ans:0},
{q:"Panel yang digunakan sebagai titik terminasi kabel jaringan agar tertata rapi di rak server disebut...", opts:["Patch Panel","Rack Server","Cable Tray","Modul Keystone"], ans:0},
{q:"Alat tangan yang digunakan untuk mengencangkan atau melepas baut/sekrup pada perakitan perangkat jaringan adalah...", opts:["Obeng","Tang Potong","Cutter","Solder"], ans:0},
{q:"Alat yang digunakan untuk memotong kabel dengan rapi sebelum dilakukan proses crimping disebut...", opts:["Cutter/Cable Cutter","Punch Down Tool","Fusion Splicer","Tone Generator"], ans:0},
{q:"Alat yang digunakan untuk melacak jalur kabel jaringan yang tertanam di dalam dinding atau tersembunyi disebut...", opts:["Toner Probe (Tone Generator and Probe)","Multimeter","Crimping Tool","Fusion Splicer"], ans:0},
{q:"Alat yang digunakan untuk mengencangkan sambungan solder pada komponen elektronik jaringan disebut...", opts:["Solder dan Timah","Obeng","Tang Kombinasi","Gunting"], ans:0},
{q:"Perlengkapan pelindung diri yang wajib digunakan saat memotong kabel fiber optik agar serpihan kaca tidak melukai adalah...", opts:["Sarung tangan dan kacamata pelindung","Helm proyek","Sepatu boots","Masker kain"], ans:0},
{q:"Tang kombinasi dalam praktik jaringan komputer biasanya digunakan untuk...", opts:["Memotong, menjepit, dan mengupas kabel","Mengukur tegangan listrik","Menyambung fiber optik","Mendeteksi sinyal WiFi"], ans:0},
{q:"Perangkat lunak atau alat yang digunakan untuk mengecek kualitas dan kecepatan koneksi internet disebut...", opts:["Speed Test","Crimping Tool","LAN Tester","Fusion Splicer"], ans:0},
{q:"Kabel yang paling umum digunakan dalam instalasi jaringan LAN di sekolah/kantor adalah...", opts:["Kabel UTP","Kabel HDMI","Kabel VGA","Kabel Audio"], ans:0},
{q:"Berikut ini yang termasuk alat kerja (tools) dalam instalasi jaringan, kecuali...", opts:["Crimping Tool","LAN Tester","Microsoft Word","Obeng"], ans:2},
{q:"Alat yang digunakan untuk membuat lubang pada dinding atau panel guna memasang kabel/pipa jaringan disebut...", opts:["Bor listrik","Tang crimping","LAN tester","Cable stripper"], ans:0},
{q:"Toolkit jaringan yang lengkap biasanya sudah mencakup alat-alat berikut, kecuali...", opts:["Crimping tool","LAN tester","Obeng set","Kalkulator ilmiah"], ans:3},
{q:"Fungsi dari cable tester pada jaringan komputer adalah...", opts:["Menguji apakah kabel terpasang dengan benar dan tidak putus","Memotong kabel UTP","Mengukur suhu perangkat","Menyambung fiber optik"], ans:0},
{q:"Alat yang digunakan untuk menyimpan dan mengelola banyak perangkat jaringan secara rapi dan terorganisir disebut...", opts:["Rack Server","Patch Cord","Konektor","Access Point"], ans:0},
{q:"Kabel pendek yang digunakan untuk menghubungkan perangkat ke patch panel atau switch disebut...", opts:["Patch Cord","Kabel Backbone","Kabel Fiber Optik","Kabel Coaxial"], ans:0},
{q:"Berikut ini adalah alat pelindung diri (K3) yang perlu diperhatikan saat bekerja dengan alat listrik jaringan, kecuali...", opts:["Sarung tangan isolasi","Sepatu berbahan konduktor listrik","Alas kaki karet (non-konduktor)","Memastikan area kerja kering"], ans:1},
{q:"Urutan kabel straight menurut standar EIA/TIA 568B pada ujung pertama adalah...", opts:["Putih Hijau - Hijau - Putih Oranye - Biru - Putih Biru - Oranye - Putih Coklat - Coklat","Hijau - Putih Hijau - Oranye - Putih Biru - Biru - Putih Oranye - Coklat - Putih Coklat","Putih Oranye - Oranye - Putih Hijau - Biru - Putih Biru - Hijau - Putih Coklat - Coklat","Coklat - Putih Coklat - Biru - Putih Biru - Hijau - Putih Hijau - Oranye - Putih Oranye"], ans:2},
{q:"Alat yang berfungsi menyediakan daya listrik cadangan sementara ketika listrik utama padam, sehingga perangkat jaringan tidak mati mendadak, disebut...", opts:["UPS (Uninterruptible Power Supply)","Stabilizer","Adaptor","Power Supply Unit"], ans:0}
];

// ===== Util: acak array (Fisher-Yates) =====
function shuffle(array) {
  const arr = array.slice();
  for (let i = arr.length - 1; i > 0; i--) {
    const j = Math.floor(Math.random() * (i + 1));
    [arr[i], arr[j]] = [arr[j], arr[i]];
  }
  return arr;
}

// Menyiapkan set soal teracak: urutan soal diacak + urutan pilihan tiap soal diacak
function buatSoalTeracak() {
  const urutanSoal = shuffle(soalAsli.map((_, i) => i));
  return urutanSoal.map(idx => {
    const item = soalAsli[idx];
    const optIdx = shuffle(item.opts.map((_, i) => i));
    const opts = optIdx.map(i => item.opts[i]);
    const ans = optIdx.indexOf(item.ans);
    return { q: item.q, opts, ans };
  });
}

let soalData = [];
let current = 0;
let score = 0;
let answered = false;
let namaSiswa = '';
let kelasSiswa = '';

const quizArea = document.getElementById('quiz-area');
const btnNext = document.getElementById('btn-next');
const btnRow = document.getElementById('btn-row');
const progressBar = document.getElementById('progress-bar');
const progressBarWrap = document.getElementById('progress-bar-wrap');
const progressText = document.getElementById('progress-text');
const hasilDiv = document.getElementById('hasil');
const startArea = document.getElementById('start-area');
const labels = ['A','B','C','D'];

const STORAGE_KEY = 'riwayat_kuis_tkj';

function ambilRiwayat() {
  try {
    return JSON.parse(localStorage.getItem(STORAGE_KEY)) || [];
  } catch (e) {
    return [];
  }
}

function simpanRiwayat(entry) {
  try {
    const data = ambilRiwayat();
    data.push(entry);
    localStorage.setItem(STORAGE_KEY, JSON.stringify(data));
    return true;
  } catch (e) {
    return false;
  }
}

function renderRiwayat() {
  const data = ambilRiwayat();
  const tbody = document.querySelector('#tabel-riwayat tbody');
  const kosong = document.getElementById('riwayat-kosong');
  tbody.innerHTML = '';
  if (data.length === 0) {
    kosong.style.display = 'block';
    return;
  }
  kosong.style.display = 'none';
  data.slice().reverse().forEach(row => {
    const tr = document.createElement('tr');
    tr.innerHTML = '<td>' + row.nama + '</td><td>' + row.kelas + '</td><td>' + row.skor + '/' + row.total + '</td><td>' + row.nilai + '</td><td>' + row.waktu + '</td>';
    tbody.appendChild(tr);
  });
}

document.getElementById('btn-clear-riwayat').addEventListener('click', () => {
  if (confirm('Hapus semua riwayat nilai di perangkat ini?')) {
    try { localStorage.removeItem(STORAGE_KEY); } catch(e) {}
    renderRiwayat();
  }
});

document.getElementById('btn-start').addEventListener('click', () => {
  namaSiswa = document.getElementById('nama').value.trim() || 'Tanpa Nama';
  kelasSiswa = document.getElementById('kelas').value.trim() || '-';

  soalData = buatSoalTeracak();
  current = 0;
  score = 0;

  startArea.classList.add('hidden');
  quizArea.classList.remove('hidden');
  btnRow.classList.remove('hidden');
  progressBarWrap.style.display = 'block';
  hasilDiv.style.display = 'none';

  renderSoal();
});

function renderSoal() {
  answered = false;
  btnNext.disabled = true;
  btnNext.textContent = (current === soalData.length - 1) ? 'Selesai & Lihat Hasil' : 'Jawaban Selanjutnya';

  const item = soalData[current];
  let html = '<div class="soal"><p class="pertanyaan">' + (current + 1) + '. ' + item.q + '</p><ul class="pilihan">';
  item.opts.forEach((opt, i) => {
    html += '<li data-idx="' + i + '"><span class="label">' + labels[i] + '.</span> ' + opt + '</li>';
  });
  html += '</ul></div>';
  quizArea.innerHTML = html;

  document.querySelectorAll('.pilihan li').forEach(li => {
    li.addEventListener('click', () => selectAnswer(li));
  });

  updateProgress();
}

function selectAnswer(li) {
  if (answered) return;
  answered = true;
  const idx = parseInt(li.dataset.idx);
  const correctIdx = soalData[current].ans;

  document.querySelectorAll('.pilihan li').forEach(el => {
    el.classList.add('locked');
    const eIdx = parseInt(el.dataset.idx);
    if (eIdx === correctIdx) el.classList.add('correct');
    else if (eIdx === idx) el.classList.add('incorrect');
  });

  if (idx === correctIdx) score++;
  btnNext.disabled = false;
}

function updateProgress() {
  const pct = (current / soalData.length) * 100;
  progressBar.style.width = pct + '%';
  progressText.textContent = 'Soal ' + (current + 1) + ' dari ' + soalData.length;
}

btnNext.addEventListener('click', () => {
  if (current < soalData.length - 1) {
    current++;
    renderSoal();
  } else {
    showHasil();
  }
});

let hasilTerakhir = null;

function showHasil() {
  progressBar.style.width = '100%';
  progressText.textContent = 'Kuis selesai!';
  quizArea.classList.add('hidden');
  btnRow.classList.add('hidden');

  const persen = Math.round((score / soalData.length) * 100);
  const waktu = new Date().toLocaleString('id-ID');

  document.getElementById('hasil-nama').textContent = namaSiswa;
  document.getElementById('hasil-kelas').textContent = kelasSiswa;
  document.getElementById('skor').textContent = score + ' / ' + soalData.length;
  document.getElementById('skor-detail').textContent = 'Nilai: ' + persen + ' — ' +
    (persen >= 80 ? 'Sangat Baik!' : persen >= 60 ? 'Cukup Baik' : 'Perlu Belajar Lagi');

  hasilTerakhir = { nama: namaSiswa, kelas: kelasSiswa, skor: score, total: soalData.length, nilai: persen, waktu: waktu };
  simpanRiwayat(hasilTerakhir);
  renderRiwayat();

  hasilDiv.style.display = 'block';
}

document.getElementById('btn-restart').addEventListener('click', () => {
  hasilDiv.style.display = 'none';
  startArea.classList.remove('hidden');
  progressBarWrap.style.display = 'none';
  progressText.textContent = '';
  document.getElementById('nama').value = '';
  document.getElementById('kelas').value = '';
});

document.getElementById('btn-download').addEventListener('click', () => {
  if (!hasilTerakhir) return;
  const csvHeader = 'Nama,Kelas,Skor,Total,Nilai,Waktu\n';
  const csvRow = [hasilTerakhir.nama, hasilTerakhir.kelas, hasilTerakhir.skor, hasilTerakhir.total, hasilTerakhir.nilai, hasilTerakhir.waktu]
    .map(v => '"' + String(v).replace(/"/g,'""') + '"').join(',');
  const blob = new Blob([csvHeader + csvRow], { type: 'text/csv;charset=utf-8;' });
  const url = URL.createObjectURL(blob);
  const a = document.createElement('a');
  a.href = url;
  a.download = 'nilai_' + hasilTerakhir.nama.replace(/\s+/g,'_') + '.csv';
  document.body.appendChild(a);
  a.click();
  document.body.removeChild(a);
  URL.revokeObjectURL(url);
});

// Muat riwayat saat halaman dibuka
renderRiwayat();
</script>

</body>
</html>
