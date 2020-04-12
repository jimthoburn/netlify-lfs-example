# netlify-lfs-example

```
$ cd netlify-lfs-example 
$ git lfs install
$ git lfs track "*.jpg" "*.jpeg" "*.png" "*.gif"
$ git add .gitattributes
$ git status
$ git commit -m "Enable Git LFS"
$ git push origin master
$ netlify link
$ netlify lm:setup

  ⠙ Provisioning Netlify Large Media
  ✔ Provisioning Netlify Large Media
  ✔ Configuring Git LFS for this site

$ git status
  .gitignore
  .lfsconfig
$ cat .lfsconfig 

[lfs]
	url = https://8b48c355-e80f-4c95-8e37-0bdb3203d48b.netlify.com/.netlify/large-media

$ cat .netlify/state.json

{
	"siteId": "8b48c355-e80f-4c95-8e37-0bdb3203d48b"
}

$ git add .
$ git commit -m "Use Netlify for LFS"  
$ git push origin master

To https://github.com/jimthoburn/netlify-lfs-example.git
   286081f..89de01d  master -> master

$ git add .
$ git commit -m "Add an example picture"

1 file changed, 3 insertions(+)
create mode 100644 chia-seeds.jpg

$ git push origin master

Uploading LFS objects: 100% (1/1), 156 KB | 0 B/s, done.                                                                                                     
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 393 bytes | 393.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/jimthoburn/netlify-lfs-example.git
   89de01d..709bce5  master -> master
$
```

<img width="1016" alt="Netlify Large Media" src="https://user-images.githubusercontent.com/926616/79077414-71998500-7cb6-11ea-9cb4-e5d915dcf4f1.png">

https://lfs-example-jimthoburn.netlify.com/chia-seeds.jpg
