### 1 install msys2 https://www.msys2.org/
### 2 install gtk https://www.gtk.org/docs/installations/windows/
```shell
pacman -S mingw-w64-x86_64-gtk4
pacman -S mingw-w64-x86_64-glade
pacman -S mingw-w64-x86_64-toolchain base-devel
```

### 3 set var
```shell
set PKG_CONFIG_PATH=C:\msys64\mingw64\lib\pkgconfig
add PATH=C:\msys64\mingw64\bin
```

### 4 set rustup default toolchain
```shell 
rustup default nightly-x86_64-pc-windows-gnu
```

### 5 build
```shell
cargo build 
```
