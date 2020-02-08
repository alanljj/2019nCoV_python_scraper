# 2019nCoV_python_scraper
This project reference by following articles:
https://blog.csdn.net/xufive/article/details/104093197
https://blog.csdn.net/weixin_35770067/article/details/104172396

## Environment
win10 64bit
python 3.7.3 with virtualenv

## installation
```python
pip install virtualenv
```

pip china mirror config if your network is too slow:
---
python模块管理 pip临时使用及永久镜像配置:
https://www.itgeeker.net/python-how-to-config-pip-mirror-in-china/
---

### create virtual env and activate
virtualenv D:\Python\Python3_2019nCoV_env
D:\Python\Python3_2019nCoV_env\Scripts\activate

### install requirements
```
pip install -r D:\git_matebook\2019nCoV_python_scraper\requirements.txt -i http://mirrors.aliyun.com/pypi/simple/ --trusted-host mirrors.aliyun.com
```

### solution for can not install mpl_toolkits.basemap
for win10 user: go to https://www.lfd.uci.edu/~gohlke/pythonlibs/#basemap, according you python version(ex. python 3.7) download basemap‑1.2.1‑cp37‑cp37m‑win_amd64.whl(size about 116M)
for ubuntu/debian user: sudo apt-get install python-mpltoolkits.basemap

```
pip install basemap‑1.2.1‑cp37‑cp37m‑win_amd64.whl
```

#### solution for ImportError: No module named matplotlib

for win10 user: pip install --upgrade matplotlib
for ubuntu/debian user: 
    sudo pip3 uninstall matplotlib
    sudo apt-get install python3-matplotlib



https://github.com/GakkiWl/china-shapefiles