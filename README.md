# python-dictionary-to-variables
```

config = {'url': "'https://www.csdn.net/nav/python?spm=1000.2115.3001.4125'",
          "numgundong": 20,
          "guize": '//div[@class="list_con"]/div/h2/a/@href',
          "laytime": 1,

          }



print(config)
for i in config:
    if type(config[i])==str:
        tmp=config[i]
        #先来一个空.不然转移字符搞死你.
        exec(i+'='+"3")
        exec(i+'=tmp')
    else:
       tmp=i+'='+str(config[i])
       exec(tmp)

print(1)

```
