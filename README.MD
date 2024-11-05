### A simple AliCloud DNS update tool

### Usage

```bash
./ddns subdomain domain
# ./ddns dev example.com #更新 dev.example.com 的解析记录为当前主机公网IP
# ./ddns dev example.com #Update DNS record of dev.example.com to current host's public IP
```

### Cron 定时任务

```bash
crontab -e
# 添加以下行到 crontab 中
# add the following line to crontab
*/10 * * * * /path/to/ddns subdomain domain
# 每10分钟更新一次 subdomain.domain 的解析记录为当前主机公网IP
# Update DNS record of subdomain.domain to current host's public IP every 10 minutes
```
