# key add
This command adds a key to get access to the gitserver.
```shell
key add ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQD6hLTCJQ0J9e3KxrG3dqZqWY/Wth9gHT6KyOgylTsmaRHKQfa1Xsdsj54S/JOM/pVqK9XK00KHxWUovvvaLlXErjOgb2PWaJa/0HNtMo80M6nXAtWcP07fSTxdvSZd+ZJC+DszkSciAZmeMKhKAb2+JT/rlCS1a1DF6GpGSsG2Pzo+iuViIywRbdik1fmDmNPyAdauQW6JG5ulBiWBph8/ElpE8DLBwaINUrN4m/tShUUIyB3wI+e5ublGlIheRkkmj66vKvcvTt93GxmLlPR/kg+oY0T8ygZZu5GKQifAVvsy2jgqlKegPHtltr7dpixrPK6b2jA3fWl6VG6f/pa9xOpSJzeimvIA6KInDkVbkwueW662aVPW7OrxUwxFsh56bUrKdpE+e7o6VByA3nAz9KBIEY9JXV/3oUoxJ7zv+vOKN/3vtep2YhianQr4Yzx9/QDlUFcYwANfljRZlQpbEvra8gyhShYC8RUGaeRQqnzJ5hDKZWNswpPyJkCAPS5d940y0R52DFENowlImuhS+QRgrLPOtTqFvkFNb2TmKRUaVXT9sa9ooGmcb/FsxBLvk0mm0yWqi+LO6FSlQwEfipOTvAVqJNeFFZVbqMbgrZczHZkbaVG6QBHQxw9qZfSWtuY7Iku6HcX6GR1+cKYdfXa4yUwy04afEi978jwV4Q== your_email@example.com
```

# key ls
This command lists all the keys which have access to the gitserver. 
```shell
key ls
```


# key rm
This command removes a key from the gitserver. It takes a number as an argument, you can find the numbers by using `key ls`.
```shell
key rm 2 
```
