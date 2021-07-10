# Script de Youtube DL

Um script simples para baixar/transferir músicas/vídeos do YouTube.

- [Script de Youtube DL](#script-de-youtube-dl)
    - [Observação](#observação)
      - [`youtube-dl`](#youtube-dl)
        - [Global](#global)
        - [Alpine Linux](#alpine-linux)
        - [Arch Linux e derivados de Arch Linux](#arch-linux-e-derivados-de-arch-linux)
        - [CentOS](#centos)
        - [Debian e derivados de Debian](#debian-e-derivados-de-debian)
        - [Fedora e derivados de Fedora](#fedora-e-derivados-de-fedora)
        - [openSUSE](#opensuse)
        - [Solus](#solus)
      - [`ffmpeg`](#ffmpeg)
        - [Variados](#variados)
        - [CentOS, Fedora e derivados de Fedora](#centos-fedora-e-derivados-de-fedora)
    - [Instruções](#instruções)

### Observação
- Funciona apenas em Linux e nos sistemas Unix, inclusive FreeBSD. Deve funcionar no WSL do Windows.
- É necessário `youTube-dl` e `ffmpeg` para a conversão dos vídeos.

#### `youtube-dl`

##### Global

```bash
pip install youtube-dl
```

##### Alpine Linux

```bash
apk update
apk add --upgrade youtube-dl
```

##### Arch Linux e derivados de Arch Linux

```bash
# pacman
sudo pacman youtube-dl

# yay - o último commit do repositório
youtube-dl-git
```

##### CentOS

Baixa/transfere [aqui](http://download-ib01.fedoraproject.org/pub/epel/8/Everything/aarch64/)

```bash
rpm -Uvh epel-release*rpm
dnf install youtube-dl
```

##### Debian e derivados de Debian

```bash
sudo apt install youtube-dl
```

##### Fedora e derivados de Fedora

```bash
sudo dnf install youtube-dl
```

##### openSUSE

```bash
sudo zypper install youtube-dl
```

##### Solus

```bash
sudo eopkg install youtube-dl
```

#### `ffmpeg`

##### Variados

```bash
# Alpine Linux
apk add --upgrade ffmpeg

# Arch Linux
sudo pacman -Syu ffmpeg

# Debian e derivados de Debian
sudo apt install ffmpeg

# FreeBSD
pkg install ffmpeg

# Mageia
urpmi ffmpeg

# openSUSE
sudo zypper install ffmpeg-4

# Solus
sudo eopkg dr Solus
sudo eopkg rr Solus
sudo eopkg ar Solus https://mirrors.rit.edu/solus/packages/unstable/eopkg-index.xml.xz
sudo eopkg install ffmpeg
```

##### CentOS, Fedora e derivados de Fedora

Baixe/transfira [aqui](http://download1.rpmfusion.org/free/fedora/).

```bash
rpm -Uvh rpmfusion-free-release-stable*rpm
dnf --enablerepo=rpmfusion-free-rawhide install ffmpeg
```

### Instruções

Após as inatalações necessárias, apenas execute o script `ytdl.py` e siga os passos. 
