# quicksilver-fix-


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
and mnemonic

```
quicksilverd keys export mainnetcüzdanadı --unarmored-hex --unsafe
```
çıkan private keyimizi keplere ekliyoruz bamm mallar içerde hayırlı olsun Ttoprak73  private key alma kodunu verdmesinden ötürü çok tşk ederim beraberce çözdük sanırım 

