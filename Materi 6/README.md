# Materi ke-6 - Kubernetes For Beginners

Melakukan login ke akun Docker Hub supaya dapat menampilkan terminal


Menjalankan perintah *ls* kemudian menjalankan perintah *kubeadm init --apiserver-advertise-address $(hostname -i)* untuk menginisialisasi gugus pada terminal pertama


Setelah melakukan inisialisasi dilanjutkan dengan menjalankan perintah *kubeadm join 192.168.0.33:6443 --token bdk9eq.z3q1b4rhpbuyhlw5 \ --discovery-token-ca-cert-hash sha256:315c1a287b01338b26c0131a9d0cd81fd1db18197fe3f779d099207191c7a68b*


Yang terakhir untuk mengatur cluster yaitu dengan menjalankan perintah *kubectl apply -n kube-system -f \ "https://cloud.weave.works/k8s/net?k8s-version=$(kubectl version | base64 |tr -d '\n')"*


Menjalankan perintah *git clone https://github.com/dockersamples/dockercoins* untuk melakukan clone repository Dockercoins


Setelah proses clone selesai dilanjutkan dengan membuka direktori Dockercoins yang telah didiclone dengan menjalankan perintah *cd ~/dockercoins* dan dilanjutkan kembali dengan menjalankan container Dockercoins dengan menjalankan perintah *docker-compose up*



Untuk melihat komposisi dari Cluster dapat menjalankan perintah *kubectl get node*


Untuk melihat info lebih lanjut mengenai node dapat menjalankan perintah *kubectl get nodes -o wide*


Untuk menampilkan info berupa YAML dapat dilakukan dengan menjalankan perintah *kubectl get no -o yaml*


Menampilkan kapasitas semua node sebagai aliran objek JSON dengan menjalankan perintah *kubectl get nodes -o json | jq ".items[] | {name:.metadata.name} + .status.capacity"*


Melihat daftar layanan Cluster

