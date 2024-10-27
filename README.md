# legacy_boilerplate_dashboard
dashboard 모니터링

# Window 구성 필요  

---

# Intellij Local 환경구성 MAC기준   

---

## tomcat 9.0 Download
https://tomcat.apache.org/download-90.cgi
```text
tomcat 8.5 apache 진형에서 지원하지 않는것으로 확인되어 
9.0 버전 사용 추후 하위버전도 9.0 사용가능한지 검증 필요

9.0.96 > Core > zip(pgp, sha512) Download
```

### tomcat custom 설치 경로 : 
```shell
~/was/apache-tomcat-9.0.96
```
### 폴더구성 : 
```shell
-rw-r--r--@  1 lswteen  staff  10244 10 27 10:18 .DS_Store
-rw-r--r--@  1 lswteen  staff  21516 10  3 19:44 BUILDING.txt
-rw-r--r--@  1 lswteen  staff   6330 10  3 19:44 CONTRIBUTING.md
-rw-r--r--@  1 lswteen  staff  58153 10  3 19:44 LICENSE
-rw-r--r--@  1 lswteen  staff   2401 10  3 19:44 NOTICE
-rw-r--r--@  1 lswteen  staff   3362 10  3 19:44 README.md
-rw-r--r--@  1 lswteen  staff   7075 10  3 19:44 RELEASE-NOTES
-rw-r--r--@  1 lswteen  staff  17016 10  3 19:44 RUNNING.txt
drwxr-xr-x@ 29 lswteen  staff    928 10  3 19:44 bin
drwxr-xr-x@ 13 lswteen  staff    416 10 27 11:10 conf
drwxr-xr-x@ 35 lswteen  staff   1120 10  3 19:44 lib
drwxr-xr-x@  8 lswteen  staff    256 10 27 11:11 logs
drwxr-xr-x@  3 lswteen  staff     96 10  3 19:44 temp
drwxr-xr-x@ 10 lswteen  staff    320 10 27 11:11 webapps
drwxr-xr-x@  3 lswteen  staff     96 10 27 10:40 work

conf : server.xml, web.xml
server.xml PORT정보, Context Path 경로 
web.xml 기본 접근파일 선언
```
### logs : 
```shell
tail -F ~/was/apache-tomcat-9.0.96/logs/catalina.out
```

### 실행
```shell
# Tomcat 서버 중지
~/was/apache-tomcat-9.0.96/bin/shutdown.sh

# Tomcat 서버 시작
~/was/apache-tomcat-9.0.96/bin/startup.sh
```

### 파일 권한 
```shell
chmod 755 /Users/lswteen/was/apache-tomcat-9.0.96/webapps/dashboard.war
```

### Intellij 설정
<img width="1439" alt="스크린샷 2024-10-27 오후 3 13 17" src="https://github.com/user-attachments/assets/e75e6426-6d55-453c-a58a-2972a00bb43e">
<img width="1436" alt="스크린샷 2024-10-27 오후 3 13 23" src="https://github.com/user-attachments/assets/94475a8b-08bd-4140-b3d2-b7c28320aa59">
