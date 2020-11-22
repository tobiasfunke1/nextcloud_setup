# nextcloud_setup

### data directory on nfs
```
# show nfs list
showmount -e x.y.z.35

# /etc/fstab entry
x.y.z.35:/volume1/nextcloud /mnt/nextcloud_nfs defaults 0 0

# create directory
mkdir /mnt/nextcloud_nfs/ncdata
chown -R www-data:www-data /mnt/nextcloud_nfs/ncdata

# move data directory
x.y.z.35:4443/?app=nc-datadir
```
