# git push

git push: untuk muat naik lokal repo ke remote repo

## Cara penggunaan git push

cara untuk guna git push untuk push lokal repo ke remote repo

```bash
git push <remote> <branch>
```

&lt;remote&gt; - nama remote repo. biasanya nama 'origin' yang digunakan

&lt;branch&gt; - nama branch yang mahu dimuat naik

## contoh arahan git push

### arahan lalai git push

contoh dibawah adalah cara umum untuk menggunakan arahan git push.

```bash
# keluar ke ranting main
git checkout main
# kemaskini lokal repo
git fetch origin main
# rebase ke origin/main
git rebase -i origin/main
# upload menggunakan git push
git push origin main
```

sumber: [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/syncing/git-push)

