Ganglia

	Ganglia adalah alat pemantauan yang dapat diskalakan dan terdistribusi untuk sistem, cluster, dan jaringan
  komputasi kinerja tinggi. Perangkat lunak ini digunakan untuk melihat statistik langsung atau rekaman yang
  mencakup metrik seperti rata-rata beban CPU atau pemanfaatan jaringan untuk banyak node. Perangkat lunak 
  Ganglia bisa digunakan untuk distribusi Linux tingkat perusahaan seperti Red Hat Enterprise Level (RHEL)
  atau CentOS. Ganglia pertama kali di buat dan digunakan  oleh Berkeley (University of California) tetapi 
  sekarang banyak digunakan juga oleh organisasi komersial dan pendidikan seperti Cray, MIT, NASA dan Twitter.
  Ganglia memiliki 3 komponen inti yaitu ganglia Monitoring Daemon (gmond), ganglia Meta Daemon (gmetad),
  ganglia PHP Web.


Ganglia Monitoring Daemon (gmond) 
  Adalah daemon multi-threaded yang berjalan pada setiap node cluster yang ingin di  pantau. Tugasnya adalah
  untuk memantau perubahan dalam host., memberi tahu perubahan yang relevan, melihat status semua node ganglia
  lainnya melalui saluran unicast atau multicast. memberikan deskripsi XML dari cluster.

Ganglia Meta Daemon (gmetad) 
  menggunakan pohon koneksi point-to-point antara node cluster. Tugasnya adalah secara berkala mengumpulkan
  kumpulan sumber data, mem-parsing XML yang dikumpulkan, menyimpan semua numerik, metrik yang mudah berubah
  ke round-robin database dan mengekspor XML yang diagregasikan melalui soket TCP ke client.


Ganglia PHP Web 
  memberikan informasi yang dikumpulkan melalui halaman web dinamis secara real time. Yang paling penting, ini
  menampilkan data Ganglia dengan cara yang berarti bagi administrator sistem dan pengguna komputer. Meskipun
  web ganglia mengunakan tampilan HTML sederhana namun ia telah berevolusi menjadi sistem yang menyimpan sejarah
  penuh warna dari semua data yang dikumpulkan.
