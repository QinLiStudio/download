# 琴理工作室下载站

> Nginx FancyIndex

```bash
# clone本项目到服务器
git clone https://github.com/QinLiStudio/download.git

# 使用docker部署
docker run -d \
  --name fancyindex \
  -v <file path>:/share \
  -v <repo path>:/theme/Nginx-Fancyindex-Theme/ \
  -p 8000:80 \
  -e "DISABLE_AUTH=true" \

  --restart always \
  fraoustin/fancyindex \

```