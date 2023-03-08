<div align="center">

# Minima Ödül Talebi & Cüzdan Yedeklemesi Nasıl yapılır?

</div>

Yapmamız gerekenlerı kısaca özetliyorum. Öncelikle Minimum 2cpu 2 ram sunucu temin ediyoruz ve içine Minima Nodunu kuruyoruz. Sonrasında MiniDappimize girip IP Reward eklentisini oraya kuruyoruz. Sonrasında Terminale Write İzinini verip, Terminale giriyoruz. Oraya mds yazıp uid alıyoruz sonrasında vault yazıp cüzdan kelimelerimizi alıyoruz. Bu aşamadan sonra ödülleri claim etmek kaldı.

<details>

<summary> 
<h2> 1) Minima Kurulumu 
</summary> </h2>

## Güncelleme ve Gerekli Dosyaları Kuralım.
```
sudo su
```
```
sudo apt update 
```
```
sudo apt upgrade
```
## Minimayı Kuralım.

```
sudo curl -fsSL https://get.docker.com/ -o get-docker.sh
```
```
sudo chmod +x ./get-docker.sh && ./get-docker.sh
```

## Minimayı Kuralım.
Mini Dappe Erişmek için Şifreniz 123 olacak bunu unutmayın!

```
docker run -d -e minima_mdspassword=123 -e minima_server=true -v ~/minimadocker9001:/home/minima/data -p 9001-9004:9001-9004 --restart unless-stopped --name minima9001 minimaglobal/minima:latest
```
```
sudo systemctl enable docker.service
```
```
sudo systemctl enable containerd.service
```
## Kurulum Bitti Şimdi Nodeu Kontrol edelim.

``docker ps`` yazın ve CONTAINER ID altındaki komutu aşağıda BURAYA yazan yer ile değiştirin. Örnek "docker logs k3msdlxc31 --follow"
```
docker ps
```
```
docker logs BURAYA --follow
```
![minimadockerps](https://user-images.githubusercontent.com/76253089/223828847-c0f0d836-92f3-489e-ae38-a616de45d600.png)

## Eğer Bu şekildeyse sorun yoktur diğer adıma geçelim.
![nodecıktısıbusekil](https://user-images.githubusercontent.com/76253089/223829381-fef586de-300d-40bb-93b5-11f1c063bbc1.png)

</details>

<details>

<summary> 
<h2> 2) MiniDappe Erişim ve Cüzdan Kelimelerini Yedekleme
</summary> </h2>

## Chromea girip yeni sekme açalım ve aşağıdaki komutla Minidappe erişelim.
Server İpinizi alttaki yazı ile değişin. Çıkan Ekrandaki yere 123 yazın.
```
https://SERVERIPNİZ:9003/
```
![image](https://user-images.githubusercontent.com/76253089/223830842-f2acbe28-df55-4716-b808-a553bef1103e.png)

## Şifreyi girdikten sonra Main Menu Tusuna basın. Karşınıza Dappler gelecektir. Bizim işimiz öncelikle terminalle. Write Tuşuna Basarak Gerekli izini verelim ve tekrar main menuye dönelim.

![image](https://user-images.githubusercontent.com/76253089/223831980-10fe3bc7-5d4b-41d6-848e-573e796139f8.png)

## Sonrasında Terminalin Üstüne 1 Kere basıp içine giricez. Bizi Alttaki gibi Siyah Ekran Karşılayacak. Buraya Alttaki Komutu yazın ve Çıkan çıktıyı tamamiyle kopyalayıp yedekleyin.

```
vault
```

![image](https://user-images.githubusercontent.com/76253089/223834160-e8636b42-79da-41a5-a88b-4f0cdd97333a.png)


## Cüzdan Yedekleme İşlemi Bu Kadardı. Şimdi Bu cüzdanımıza Ödüllerimizi Talep Edicez. Bir sonraki aşamaya geçin.

</details>

<details>

<summary> 
<h2> 3) Ödülleri Cüzdanımıza Talep Etme
</summary> </h2>

## Altta verdiğim Linke girip Incentive Program Rewards 2.15.1 MiniDappini indirmemiz gerekiyor. İşaretledigim yere basarak indirin.
![image](https://user-images.githubusercontent.com/76253089/223836309-d043fdae-52fa-4ce4-9a1d-da1fb5e93a52.png)
