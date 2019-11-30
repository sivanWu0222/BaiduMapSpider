# BaiduMapSpider
线路爬取


## json使用

> json.loads() 参数是一个str,可以将str转换为dict
> json.load() 参数是一个文件对象，可以将文件句柄转换为一个dict

```python
import json
import requests
url = 'http://www.baidu.com'
json.loads(requests.get(url).text)
json.load(open('1.file', 'r'))
```

## csv 库的使用

### 写csv文件

```python
import csv
if __name__ == '__main__':
    with open('result.csv', "a+", newline='') as f:
        writer = csv.writer(f, delimiter=':')  # delimiter用于csv文件中分隔符的显示,默认是,
        writer.writerow(['1', '2', 3])
```



