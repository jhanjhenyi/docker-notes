# Nginx

## 執行一個 Web Server

```bash
docker run -it --rm -d -p 8080:80 --name web nginx
```

開啟 http://localhost:8080

## 建立一個 Nginx image

Nginx 預設會用 `/usr/share/nginx/html` 資料夾裡的檔案來提供服務，所以需要把 HTML 檔案放進這個資料夾裡

```bash
docker build -t webserver .
docker run -it --rm -d -p 8080:80 --name web webserver
```
