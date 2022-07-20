# nimbus2022
The UVIS app will be substituted by this app.

<br>

---

## Docker, docker-compose 버전 (참고)
```bash
> docker —version && docker-compose —version
Docker version 20.10.16, build aa7e414
docker-compose version 1.29.2, build 5becea4c
```

<br>

---
## 개발 환경에서 app 실행 방법
### 1. git clone
```bash
❯ git clone https://github.com/toughhyeok/nimbus2022.git
Cloning into 'nimbus2022'...
remote: Enumerating objects: 126, done.
remote: Counting objects: 100% (126/126), done.
remote: Compressing objects: 100% (90/90), done.
remote: Total 126 (delta 60), reused 89 (delta 28), pack-reused 0
Receiving objects: 100% (126/126), 19.74 KiB | 2.82 MiB/s, done.
Resolving deltas: 100% (60/60), done.
```

<br>

### 2. docker build
```bash
❯ docker-compose build
```

<br>

### 3. docker-compose up
```bash
❯ docker-compose up
```

에러 발생 시 github Issues에 생성 (에러 코드 포함) 

```bash
❯ docker-compose up
nimbus2022_db_1 is up-to-date
Starting nimbus2022_app_1 ... done
Attaching to nimbus2022_db_1, nimbus2022_app_1
db_1   | The files belonging to this database system will be owned by user "postgres".
...
app_1  | July 20, 2022 - 11:59:43
app_1  | Django version 3.2.14, using settings 'app.settings'
app_1  | Starting development server at http://0.0.0.0:8000/
app_1  | Quit the server with CONTROL-C.
```

<br>

### 4. 웹 브라우저에서 http://localhost:8000/ 접속
<img width="536" alt="image" src="https://user-images.githubusercontent.com/88708976/179977048-b6eb00a8-900b-4ae0-9caf-46c18e59ec27.png">

<br>

### 5. Swagger 접속 (api docs)
[http://localhost:8000/api/docs/](http://localhost:8000/api/docs)

<br>

<img width="1482" alt="image" src="https://user-images.githubusercontent.com/88708976/179977270-d667fc19-b9b6-4caf-ae54-b5bc44d1e5e1.png">
(참고) `api-schema`는 Swagger 화면 구성을 위해 필요한 것으로 실제 api로 사용되지 않음

<br>

### 6. api test

### 7. admin 페이지 접속
[http://localhost:8000/admin/](http://localhost:8000/admin/)

관리자 계정은 카톡으로 물어보시면 됩니당

<br>

<img width="1512" alt="image" src="https://user-images.githubusercontent.com/88708976/179978920-ef066403-3d01-46c1-b18d-1d795e16a17d.png">

