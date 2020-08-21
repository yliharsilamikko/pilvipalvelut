# Pilvipalvelut (Docker)

https://kodekloud.com/p/docker-labs


## Tavoitteet

* Opiskella Dockerin käyttöä/komentoja
* Dockerin appin luonti
* Appin julkaisu pilveen (Heroku)
  - Node + Mongo + Express
* "Harjoitustyö"


## Docker omalle koneelle

1. WSL2 (vaati vähän vaivaa, nopein, tulevaisuuden työkalu)
2. Docker Desktop for Windows 
 * helpoin
 * suositeltu tälle kurssille
 * vaati että hyper-v on päällä
 * Vaatii Windows 10 pro / ilmeisesti home versiolla 2020 toimii
3. Virtualbox / VmWare - esim. ubuntu-server
  * dockerin asennus (apt-get install docker antaa mahdollisesti vanhan version)
  
## Hyödyllisiä Docker komentoja

### Lataa image
* docker pull ubuntu

### Käynnistä container imagesta
* docker run -it ubuntu
* -it menee containerin terminaaliin

### Käynnistä pysähtynyt container terminaalissa
* docker start -ai containerin_nimi tai ID

### Poista image
* docker image rm imagen_nimi tai ID
* docker image prune -a









