# extract-apkm-sigs
Extract the individual .apk signatures from within an .apkm bundle.

This does not verify correctness of the signatures, only that they match each other.
If no certificate fingerprint is publicly available, you can run this script on any old .apks you can get hold of from the same developer.

### Install:
```
curl https://raw.githubusercontent.com/morkeltry/extract-apkm-sigs/refs/heads/main/./extract-apkm-sigs >extract-apkm-sigs
chmod +x extract-apkm-sigs
```

### Run:
`./extract-apkm-sigs <.apkm file> <output dir>`

#### Dependencies
You will need a JRE and apksigner, eg:
```
sudo apt install openjdk-21-jre-headless
sudo apt install apksigner
```


