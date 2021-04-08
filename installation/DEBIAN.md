<h3>Préparer un média d'installation à partir de l'image Debian</h3>
<p>debian-live-10.8.0-amd64-standard+nonfree.iso (testé)</p>
<p>debian-live-10.9.0-amd64-standard+nonfree.iso</p>
<p>Lien pour télécharger: <a href="https://cdimage.debian.org/cdimage/unofficial/non-free/images-including-firmware/current-live/amd64/iso-hybrid/">https://cdimage.debian.org/cdimage/unofficial/non-free/images-including-firmware/current-live/amd64/iso-hybrid/</a></p>


<p><b>Noyaux testés:</b></p>

```bash
~$ dpkg --list | grep linux-image
ii  linux-image-4.19.0-14-amd64        4.19.171-2           amd64    Linux 4.19 for 64-bit PCs (signed)
ii  linux-image-4.19.0-16-amd64        4.19.181-1           amd64    Linux 4.19 for 64-bit PCs (signed)
ii  linux-image-5.10.0-0.bpo.4-amd64   5.10.19-1~bpo10+1    amd64    Linux 5.10 for 64-bit PCs (signed)
ii  linux-image-amd64                  5.10.19-1~bpo10+1    amd64    Linux for 64-bit PCs (meta-package)
```

<p><b>Dépôts sources:</b></p>

```bash
~$ cat /etc/apt/sources.list
deb http://deb.debian.org/debian buster main non-free contrib
# deb-src http://deb.debian.org/debian buster main non-free contrib

deb http://security.debian.org/debian-security buster/updates main contrib non-free
# deb-src http://security.debian.org/debian-security buster/updates main contrib non-free

deb http://deb.debian.org/debian buster-updates main contrib non-free
# deb-src http://deb.debian.org/debian buster-updates main contrib non-free

deb http://deb.debian.org/debian buster-backports main contrib non-free
```

<p><b>Activer buster-backports dans les dépôts pour mise à jour noyau:</b></p>

```bash
sudo apt update
sudo apt install -t buster-backports linux-image-amd64
sudo apt install -t buster-backports firmware-linux firmware-linux-nonfree
```

<p><b>Installation:</b></p>

```bash
sudo apt update
sudo apt upgrade
sudo apt install locales
```
