[General]
bypass-system = true
skip-proxy = 192.168.0.0/16,10.0.0.0/8,172.16.0.0/12,localhost,*.local
tun-excluded-routes = 10.0.0.0/8, 100.64.0.0/10, 127.0.0.0/8, 169.254.0.0/16, 172.16.0.0/12, 192.0.0.0/24, 192.0.2.0/24, 192.88.99.0/24, 192.168.0.0/16, 198.51.100.0/24, 203.0.113.0/24, 224.0.0.0/4, 255.255.255.255/32, 239.255.255.250/32
dns-server = 119.29.29.29,114.114.114.114,223.5.5.5,system
fallback-dns-server = system
ipv6 = false
prefer-ipv6 = false
dns-fallback-system = false
dns-direct-system = false
icmp-auto-reply = true
always-reject-url-rewrite = false
private-ip-answer = false
hijack-dns = 8.8.8.8:53,8.8.4.4:53,1.1.1.1:53,1.0.0.1:53,9.9.9.9:53,208.67.222.222:53,208.67.220.220:53,223.5.5.5:53,223.6.6.6:53,119.29.29.29:53,114.114.114.114:53
[Proxy Group]
加密货币 = select,🇯🇵JP
影音平台 = select,🇭🇰HK
AI = select,🇯🇵JP
TikTok = select,🇯🇵JP
社交媒体 = select,🇭🇰HK
谷歌 = select,🇭🇰HK
其他 = select,🇭🇰HK
漏网之鱼 = select,🇭🇰HK
🇺🇸US = url-test,interval=300,tolerance=100,timeout=5,url=http://www.gstatic.com/generate_204,policy-regex-filter=🇺🇸|US|USA|America|america|United States|美国|凤凰城|洛杉矶|西雅图|芝加哥|纽约|沪美|美
🇯🇵JP = url-test,policy-select-name=🇯🇵 JAPAN 11,interval=300,tolerance=100,timeout=5,url=http://www.gstatic.com/generate_204,policy-regex-filter=🇯🇵|JP|Japan|japan|Tokyo|tokyo|日本|东京|大阪
🇹🇼TW = url-test,policy-select-name=🇨🇳 TAIWAN 03,interval=300,tolerance=100,timeout=5,url=http://www.gstatic.com/generate_204,policy-regex-filter=🇹🇼|TW|TWN|Taiwan|Taipei|taiwan|台湾|台灣|台北|台中|新北|彰化
🇭🇰HK = url-test,policy-select-name=🇭🇰 HONG KONG 19,interval=300,tolerance=100,timeout=5,url=http://www.gstatic.com/generate_204,policy-regex-filter=🇭🇰|HK|Hong|hong|香港|深港|沪港|京港|港
[Rule]
RULE-SET,https://raw.githubusercontent.com/LingJingMaster/Shadowrocket-Rules/refs/heads/main/ApplePush.list,DIRECT
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/BlockHttpDNS/BlockHttpDNS.list,REJECT
RULE-SET,https://raw.githubusercontent.com/AceyDeng/Acey-s-/main/Grok_Intelligence.list,AI
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Twitter/Twitter.list,社交媒体
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/TikTok/TikTok.list,TIKTOK
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/PayPal/PayPal.list,🇺🇸US
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Spotify/Spotify.list,影音平台
RULE-SET,https://raw.githubusercontent.com/AceyDeng/Acey-s-/main/HK_Banks.list,DIRECT
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Cryptocurrency/Cryptocurrency.list,加密货币
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Line/Line.list,社交媒体
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Discord/Discord.list,社交媒体
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Instagram/Instagram.list,社交媒体
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Threads/Threads.list,社交媒体
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Facebook/Facebook.list,社交媒体
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Telegram/Telegram.list,社交媒体
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Pinterest/Pinterest.list,其他
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Reddit/Reddit.list,其他
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Snap/Snap.list,其他
RULE-SET,https://raw.githubusercontent.com/AceyDeng/Acey-s-/main/yahoo.list,其他
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/GitHub/GitHub.list,其他
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/GitLab/GitLab.list,其他
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Atlassian/Atlassian.list,其他
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/AOL/AOL.list,其他
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Wikipedia/Wikipedia.list,其他
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Claude/Claude.list,AI
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Gemini/Gemini.list,谷歌
RULE-SET,https://raw.githubusercontent.com/AceyDeng/Acey-s-/main/Gamma.list,谷歌
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/OpenAI/OpenAI.list,AI
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/YouTube/YouTube.list,影音平台
RULE-SET,https://raw.githubusercontent.com/AceyDeng/Acey-s-/main/Perplexity.list,AI
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Google/Google.list,谷歌
DOMAIN-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Apple/Apple_Domain.list,DIRECT
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Apple/Apple.list,DIRECT
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Netflix/Netflix.list,影音平台
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Whatsapp/Whatsapp.list,社交媒体
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/SteamCN/SteamCN.list,DIRECT
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Steam/Steam.list,DIRECT
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/ChinaMax/ChinaMax.list,DIRECT
DOMAIN-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/ChinaMax/ChinaMax_Domain.list,DIRECT
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Global/Global.list,其他
DOMAIN-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Global/Global_Domain.list,漏网之鱼
RULE-SET,https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/Shadowrocket/Lan/Lan.list,DIRECT
GEOIP,CN,DIRECT
FINAL,漏网之鱼

[Host]
*.in-addr.arpa = server:system
*.ip6.arpa = server:system
*.local = server:system
localhost = 127.0.0.1

[URL Rewrite]
'^https?://(www.)?g.cn' 'https://www.google.com' 302
'^https?://(www.)?google.cn' 'https://www.google.com' 302
