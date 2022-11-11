# Exorde Labs

Official :
>- [GITHUB ](https://github.com/exorde-labs/ExordeModuleCLI)
>- [TWITTER ](https://twitter.com/ExordeLabs)
>- [DISCORD ](https://discord.gg/exordelabs)

Explorer:

>- [explorer ](https://about:blank#blocked)

<H1>TAHAP INSTALISASI</H1>

Install Docker

```
sudo apt update -y && sudo apt install apt-transport-https ca-certificates curl software-properties-common -y && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add - && sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable" && sudo apt install docker-ce
```

Install Screen

```
sudo apt install -y build-essential libssl-dev libffi-dev git curl screen
```
Download Bahan

```
git clone https://github.com/exorde-labs/ExordeModuleCLI.git
```

Install

Edit localConfig.json version 1.3.1 ganti 1.3.2
```
cd ExordeModuleCLI
nano localConfig.json 
```
Jika sudah jangan lupa save CTRL  X Y ENTER
```
Lanjut Build

```
cd ExordeModuleCLI
docker build -t exorde-cli .
```
Jalankan Screen dan mulai Node
```
screen -S exorde
```

```
docker run -it exorde-cli -m Address0x -l 2
```

Ganti Address0x dengan address metamask mu(WalletBaru)

Contoh:

docker run -it exorde-cli -m 0x0000000000000000000000000000000000DEAD -l 2

Tonton
Di tunggu bisa, close juga bisa….
Gunakan CTRL+A+D untuk close, untuk cek kembali gunakan
```
screen -Rd exorde
```
