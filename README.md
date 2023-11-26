# Microservices
(adım 1) docker kurulu değil ise "https://www.docker.com/get-started/" buradan docker indir
(adım 2) docker kurulumu yapıldıktan sonra cmd ye "docker volume create portainer_data" yazıp çalıştır
(adım 3) ardından "docker run -d -p 8000:8000 -p 9443:9443 --name portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce:latest" cmd de çalıştır 
kurulumlar yapıldıktan sonra "http://localhost:9000/#!/home" adresinden containerslere bakabilirsin 
eğer site açılmıyorsa adım 2 de ki komut yerine "docker run -d -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock:z portainer/portainer" çalıştırabilirsin
