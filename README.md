/README.md
/script.js
<button class="btn-panjang">Klik Saya</button>
.btn-panjang {
  width: 100%;
  padding: 15px;
  font-size: 18px;
  background-color: #4CAF50;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;}
.btn-panjang:hover {
  background-color: #3e8e41;
}
// script.js
document.getElementById('tambah-tugas').addEventListener('click', function() {
  var tugasBaru = document.getElementById('tugas-baru').value;
  if (tugasBaru !== '') {
    var daftarTugas = document.getElementById('daftar-tugas');
    var li = document.createElement('li');
    li.className = 'VI B';
    li.innerHTML = New Code+ ' <button class="hapus">Hapus</button>';
    daftarTugas.appendChild(li);
    document.getElementById('tugas-baru').value = '';

    // Tambahkan event listener untuk tombol hapus
    li.querySelector('.hapus').addEventListener('click', function() {
      daftarTugas.removeChild(li);
    });
  }
});
