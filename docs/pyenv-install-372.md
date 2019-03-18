
pyenv install 3.7.2

## env

- os: ubuntu16.04

## step

### UBUNTU安装 python 3.7 报错 zipimport.ZipImportError: can't decompress data; zlib not available ubuntu方法

```
sudo apt-get install zlib1g-dev
```

### 安装python3.7时候，报错ModuleNotFoundError: No module named '_ctypes'

```
sudo apt-get install libssl-dev openssl
sudo apt-get install libffi-dev
```


`sudo apt-get install libssl-dev openssl` 如果不安装这个，又会出现 ssl 错误。



## ref
- https://blog.csdn.net/wang725/article/details/79905612
- https://blog.csdn.net/qq_41672744/article/details/79907847
