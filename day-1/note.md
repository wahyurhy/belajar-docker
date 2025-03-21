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