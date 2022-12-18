# quicksilver-fix-
```
sudo apt install curl build-essential git wget jq make gcc tmux -y
```
```
rm -rvf /usr/local/go/
wget https://golang.org/dl/go1.19.3.linux-amd64.tar.gz
sudo tar -C /usr/local -xzf go1.19.3.linux-amd64.tar.gz
cat <<EOF >> ~/.profile
export GOROOT=/usr/local/go
export GOPATH=$HOME/go
export GO111MODULE=on
export PATH=$PATH:/usr/local/go/bin:$HOME/go/bin
EOF
source ~/.profile
go version
```


```
git clone https://github.com/ingenuity-build/quicksilver && cd quicksilver
git fetch origin --tags
git checkout v1.0.0
make install
```


```
quicksilverd config chain-id quicksilver-1
quicksilverd config keyring-backend test
```

```
quicksilverd init <moniker-name> --chain-id=quicksilver-1
```
```
quicksilverd keys add cüzdanadı --interactive
```
buraya mnemoniclerimizi yazıyoruz ne şifre girdiysek onceden hatırlıyorsanız onu yazıyoruz 2 defa cüzdanı eklıyor kontrol edin mainnet adresi olduğunu kaydettiğinizle

```
quicksilverd keys export mainnetcüzdanadı --unarmored-hex --unsafe
```
çıkan private keyimizi keplere ekliyoruz bamm mallar içerde hayırlı olsun Ttoprak73  private key alma kodunu verdmesinden ötürü çok tşk ederim beraberce çözdük sanırım 

tamam buraya kadar geldik malı aldık elimiz değmişken stakede yapalım malum cüzdandan keplr den stake yapamıyoruz ama burdan oluyro

alttaki adres benim validatorun.
```
quicksilverd tx staking delegate quickvaloper1jhv0ejjud3h8mr7v72mwmx9xeyzz84mwm2fzye miktar000000uqck --from=cüzdanadı --node http://75.119.144.167:26657 --chain-id=quicksilver-1 --gas=250000
```
# https://t.me/gokhan_molla  özelden adresinizi atın size stake yapabilmeniz için bakiye atayım arkadaşlar.
