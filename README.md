
### 使用库
- [itchat][2] - 微信个人号接口
- [requests][3] - 网络请求库
- [beautifulsoup4][4] - 解析网页
- [APScheduler][5] - 定时任务


```
itchat.auto_login()
itchat.send(today_msg, toUserName=name_uuid)
```


## 项目运行

### 安装依赖

使用 pip install -r requirements.txt 安装所有依赖

### 参数配置
config.yaml
```
#每天的几点开始发送信息
alarm_timed: '9:30'
#图灵key
tuling_key: '359a013d925040a28e6191831f9f36bc'
girlfriend_infos:
  -
    #女友微信昵称
    wechat_name: '动霸tua'
    #女友所在城市
    city_name: '成都'
    # 从那天开始勾搭的（可空）
    start_date: '2012-12-9'
    # 短句的最后留言（可空）
    sweet_words: '来自最爱你的我。'

    #如果你有多个人需要发送，则参照这个样式，复制即可
    #如不需要，则删除或注解下面所有的数据
    # wechat_name: '陈老师'
    # city_name: '朝阳区'
    # start_date: '2018-11-11'
    # sweet_words: '来自你俊美的老公。'
```

### 开始运行
```
python TLwechat.py
```

