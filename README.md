# 阻止 HTTPDNS 服务

# YY语音
domain-rule:
  - yyapp-httpdns.gslb.yy.com: reject
  - union-httpdns.gslb.yy.com: reject
  - httpdns-v6.gslb.yy.com: reject

# 虎牙
url-regex-rule:
  - "^http:\/\/cdn\.wup\.huya\.com\/launch\/queryHttpDns": reject

# 微信
domain-rule:
  - dns.weixin.qq.com: reject
  - dns.weixin.qq.com.cn: reject
  - aedns.weixin.qq.com: reject

# QQ音乐
domain-rule:
  - httpdns.kg.qq.com: reject
url-regex-rule:
  - "^http:\/\/182\.256\.116\.116\/d": reject

# 哔哩哔哩
domain-rule:
  - httpdns.bilivideo.com: reject
url-regex-rule:
  - "^http:\/\/47\.101\.175\.206\/resolve": reject
  - "^http:\/\/47\.100\.123\.169\/resolve": reject
  - "^http:\/\/120\.46\.169\.234\/resolve": reject
  - "^http:\/\/121\.36\.72\.124\/resolve": reject

# 小米
domain-rule:
  - httpdns.browser.miui.com: reject
  - resolver.msg.xiaomi.net: reject

# 阿里巴巴
domain-rule:
  - httpdns.alicdn.com: reject
  - httpdns-api.aliyuncs.com: reject
  - httpdns-sc.aliyuncs.com: reject

# 淘宝
domain-rule:
  - httpdns.danuoyi.tbcache.com: reject

# 百度
domain-rule:
  - httpdns.baidu.com: reject
  - httpsdns.baidu.com: reject
  - httpdns.bcelive.com: reject
  - httpdns.baidubce.com: reject

# 微博
domain-rule:
  - dns.weibo.cn: reject
ip-cidr-rule:
  - "39.97.130.51/32": reject
  - "39.97.128.148/32": reject
url-regex-rule:
  - "^http:\/\/api\.weibo\.cn\/2\/httpdns\/config": reject
  - "^http:\/\/api\.weibo\.cn\/httpdns\/config": reject

# 爱奇艺
domain-rule:
  - httpdns.aiqiyi.com: reject
url-regex-rule:
  - "^http:\/\/47\.100\.225\.72\/dnsresolve": reject

# 快手
domain-rule:
  - kdns.kuaishou.com: reject

# 拼多多
domain-rule:
  - httpdns.pinduoduo.com: reject

# 抖音
domain-rule:
  - httpdns.douyin.com: reject

# 美团
domain-rule:
  - httpdns.meituan.com: reject

# 快递
domain-rule:
  - httpdns.kdniao.com: reject

# 京东
domain-rule:
  - httpdns.jd.com: reject
  - resolve.jd.com: reject

# 搜狐
domain-rule:
  - httpdns.sohu.com: reject

# 腾讯视频
domain-rule:
  - httpdns.v.qq.com: reject

# 网易云音乐
domain-rule:
  - httpdns.music.163.com: reject
  - music.163.com: reject
  - dns.music.163.com: reject

# 支付宝
domain-rule:
  - httpdns.alipay.com: reject
  - httpdns.alipayobjects.com: reject

# 网易新闻
domain-rule:
  - httpdns.news.163.com: reject

# 其他域名
domain-rule:
  - dns1.chinatelecom.com: reject
  - dns2.chinatelecom.com: reject
  - resolver1.114dns.com: reject
  - resolver2.114dns.com: reject
  - cloudflare-dns.com: reject

# 禁止所有HTTPDNS解析请求
url-regex-rule:
  - "^http:\/\/.*\/httpdns": reject
  - "^https:\/\/.*\/httpdns": reject
