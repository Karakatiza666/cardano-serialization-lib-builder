https://github.com/Emurgo/cardano-serialization-lib/blob/master/README.rst#building

# Building

If you need to install Rust, do the following:
```
   curl https://sh.rustup.rs -sSf | sh -s -- -y
   echo 'export PATH=$HOME/.cargo/bin/:$PATH' >> $BASH_ENV
   rustup install stable
   rustup target add wasm32-unknown-unknown --toolchain stable
   curl https://rustwasm.github.io/wasm-pack/installer/init.sh -sSf | sh
```
To build this repository, do the following:

```
   git submodule update --init --recursive
   nvm use
   nvm install
   npm install
   npm run rust:build-nodejs
```
# Testing
```
   npm run rust:test
```