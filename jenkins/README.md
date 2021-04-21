# Jenkins

[Jenkins 官網](https://www.jenkins.io/)

## 在本機環境執行

先至 https://hub.docker.com/r/jenkins/jenkins 參考最新教學

執行指令將 Jenkins Server 執行起來

```bash
docker run -d -v jenkins_home:/var/jenkins_home -p 8080:8080 -p 50000:50000 --name jenkins jenkins/jenkins:lts
```

開啟 http://localhost:8080，會看到如下畫面

![第一次進入 Jenkins 的畫面](img/jenkins_1.png)

會發現它需要輸入密碼來解鎖，這密碼可以從 Log 獲得

![Jenkins Console Log](img/jenkins_2.png)

接下來會進入安裝畫面，這部分就看個人需求，可以先依照建議做安裝

![Customize Jenkins](img/jenkins_3.png)

安裝完後會進入建立 Admin User 的環節

![Create First Admin User](img/jenkins_4.png)

![Instance Configuration](img/jenkins_5.png)

![Jenkins is ready](img/jenkins_6.png)

![Welcom come to Jenkins](img/jenkins_7.png)
