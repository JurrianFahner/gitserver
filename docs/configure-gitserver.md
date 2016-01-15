# Get started with gitserver

The first thing you want to do is start the gitserver, it's just a one liner.

```bash
docker run -d -p 2222:22 --restart always --name devteam ensignprojects/gitserver
```

## [Add keys](./useful-commands/Command key.md) for the members of the development team
For each member you can add their keys.

```bash
docker exec -it devteam key add [key]
```

Full example:
```bash
docker exec -it devteam key add ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQD6hLTCJQ0J9e3KxrG3dqZqWY/Wth9gHT6KyOgylTsmaRHKQfa1Xsdsj54S/JOM/pVqK9XK00KHxWUovvvaLlXErjOgb2PWaJa/0HNtMo80M6nXAtWcP07fSTxdvSZd+ZJC+DszkSciAZmeMKhKAb2+JT/rlCS1a1DF6GpGSsG2Pzo+iuViIywRbdik1fmDmNPyAdauQW6JG5ulBiWBph8/ElpE8DLBwaINUrN4m/tShUUIyB3wI+e5ublGlIheRkkmj66vKvcvTt93GxmLlPR/kg+oY0T8ygZZu5GKQifAVvsy2jgqlKegPHtltr7dpixrPK6b2jA3fWl6VG6f/pa9xOpSJzeimvIA6KInDkVbkwueW662aVPW7OrxUwxFsh56bUrKdpE+e7o6VByA3nAz9KBIEY9JXV/3oUoxJ7zv+vOKN/3vtep2YhianQr4Yzx9/QDlUFcYwANfljRZlQpbEvra8gyhShYC8RUGaeRQqnzJ5hDKZWNswpPyJkCAPS5d940y0R52DFENowlImuhS+QRgrLPOtTqFvkFNb2TmKRUaVXT9sa9ooGmcb/FsxBLvk0mm0yWqi+LO6FSlQwEfipOTvAVqJNeFFZVbqMbgrZczHZkbaVG6QBHQxw9qZfSWtuY7Iku6HcX6GR1+cKYdfXa4yUwy04afEi978jwV4Q== someone of your devteam
```

## [Create](./useful-commands/Command repo.md) repository
```bash
docker exec -it devteam repo create project
```

## The server is now ready
The repo is ready for use. If you understand git, then you know what to do. If you are new to git, you need to know how to access your gitserver.
