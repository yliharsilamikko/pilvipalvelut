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

### Näytä imaget / containerit
* docker image ls
* docker container ls -a

### Käynnistä container imagesta
* docker run -it ubuntu
* -it menee containerin terminaaliin

### Käynnistä pysähtynyt container terminaalissa
* docker start -ai containerin_nimi tai ID

### Poista image
* docker image rm imagen_nimi tai ID
* docker image prune -a

### Käännä image Dockerfile:stä samassa kansiossa
* docker build -t sleepy:1 .    <- huomaa piste lopussa, joka viittaa nykyiseen kansioon

### Docker run parametreja
* -it     -> käynnistä docker terminaalitilassa
* --rm    -> poista container kun se pysähtyy
* -d      -> käynnistä detach moodissa, ajaa dockeria taustalla
* -p 8080:80     -> ohjaa containerin portti 80 ulos porttiin 8080, jolloin esim selaimella saa otettua yhteyden osoitteeseen localhost:8080

## Tunnilla tehtiin
* Docker lab 1 & 2

## Tehtävä toiselle kerralle
* asenna Docker-ympäristö omalle koneelle

## 2. Tunnilla tehtiin
* https://github.com/yliharsilamikko/pipa-exercise
* Dockerfile, imagen buildaus, CMD, ENTRYPOINT
* Docker lab 3 & 4


## VI/VIM komentoja
* vi filename.txt  -avaa tiedosto

* vi:n sisällä
* I -> mene insert moodiin, jossa voi kirjoittaa
* ESC -> poistu insert moodista
* :q -> sammuta tallentamatta
* :q! -> sammuta tallentamatta (pakota sammutus vaikka muutoksia)
* :w -> tallenna
* :wq -> tallenna ja sulje
