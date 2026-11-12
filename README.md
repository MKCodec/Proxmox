> ### Instalação ###

```sh
apt update && apt install -y git git-lfs
git lfs install
cd /var/lib/vz/dump/
git clone https://github.com/MKCodec/Proxmox.git
cd /var/lib/vz/dump/Proxmox/
git lfs pull
mv * /var/lib/vz/dump/
cd /var/lib/vz/dump/
rm -rf Proxmox
pct restore 101 vzdump-lxc-101-2026_11_11-23_06_33.tar.zst --storage local-lvm
```
