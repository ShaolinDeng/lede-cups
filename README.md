# lede-cups

git clone https://github.com/ShaolinDeng/openwrt.git


cd source

echo "src-git cups https://github.com/ShaolinDeng/lede-cups.git" >> feeds.conf.default

./scripts/feeds update -a

./scripts/feeds install -a

make menuconfig (set Network->Printing->cups as "*")

make

