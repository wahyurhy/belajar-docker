# informasi dari docker
`docker info`

# versi docker
`docker version`

# lihat images yang sudah pernah diinstall
`docker images`

# lihat daftar container yang ada di komputer kita
`docker container ls` atau bisa dengan `docker ps`
## lihat daftar container all, mau yang running maupun tidak running
`docker container ls --all`

# membuat container dari image yang sudah terinstall
`docker container create --name <namaYangKitaIngin> <image>:<tag>`

# menjalankan container
`docker container start <namaContainer>`
## sudah bisa berjalan, tapi portnya masih belum di expose, sehingga tidak dapat digunakan dari luar docker
### cara expose portnya lakukan: 
`docker container create --name <namaContainer> -p <portYangAkanDiExposePublic>:<portInternalDockerContainer> <image>:<tag>`

# menghapus container
`docker container rm <namaContainer>`
## note: harus dihentikan dulu container-nya jika masih berjalan.
### cara stop container yang berjalan: `docker container stop <namaContainer>`
#### kalau mau stop lebih dari satu container yang berjalan lakukan: `docker container stop <namaContainer> <namaContainerLainnyaDipisahkanSpasi>`