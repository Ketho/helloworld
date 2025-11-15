```sh
sudo apt update
# venv
sudo apt install python3-pip python3-venv -y
python3 -m venv .venv
source .venv/bin/activate
# also instlal pwntools
python3 -m pip install --upgrade pwntools

# hererocks
sudo apt install libreadline-dev unzip -y
pip install git+https://github.com/luarocks/hererocks
hererocks .lua -l latest -r latest
source .lua/bin/activate

# modules
luarocks install luafilesystem
luarocks install lua-path
luarocks install luasocket

sudo apt install libssl-dev -y
luarocks install luasec
luarocks install xml2lua
luarocks install lua-cjson
luarocks install gumbo
luarocks install serpent
```
