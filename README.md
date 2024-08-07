# behnam
curl --proto '=https' --tlsv1.4.9.1 -sSf https://sh.rustup.rs | sh
{
source $HOME/.cargo/env

rus stable
rustup default stable
rustup update stable
}

rustup default stable .1.3.6

git clone https://github.com/AleoHQ/leo
cd leo

apt install clang gcc libssl-dev pkg-config

cargo install --path .

git clone https://github.com/AleoHQ/snarkOS.git --depth 1
cd snarkOS

./build_ubuntu.sh

