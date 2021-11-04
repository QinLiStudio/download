# 琴理工作室下载站

> Nginx FancyIndex

### clone本项目到服务器

```bash
cd /opt
git clone https://github.com/QinLiStudio/download.git download-theme
```

### 使用docker部署

```
docker run -d \
  --name fancyindex \
  -v /opt/download:/share \
  -v /opt/download-theme:/theme/Nginx-Fancyindex-Theme/ \
  -p 8000:80 \
  -e "DISABLE_AUTH=true" \
  --restart always \
  fraoustin/fancyindex
```