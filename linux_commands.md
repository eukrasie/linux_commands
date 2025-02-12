# Linux 명령어 정리

## 1. curl (데이터 전송)

`curl`은 다양한 프로토콜(HTTP, FTP 등)을 사용하여 데이터를 전송하는 명령어입니다.

### 사용법

#### 1) 웹 페이지 요청
```sh
curl https://example.com
```
> 웹 페이지의 HTML 소스를 가져옵니다.

#### 2) 파일 다운로드
```sh
curl -O https://example.com/file.zip
```
> `-O` 옵션을 사용하면 원래 파일 이름으로 저장됩니다.

#### 3) API 요청 (GET)
```sh
curl -X GET "https://api.example.com/data"
```
> API 서버에서 데이터를 가져옵니다.

#### 4) API 요청 (POST)
```sh
curl -X POST "https://api.example.com/data" -H "Content-Type: application/json" -d '{"key":"value"}'
```
> JSON 데이터를 전송합니다.

## GitHub에 업로드하는 방법

#### 1) Git 저장소 초기화
```sh
git init
```

#### 2) 파일 추가 및 커밋
```sh
git add linux_commands.md
git commit -m "Add Linux commands documentation"
```

#### 3) 원격 저장소 연결
```sh
git remote add origin https://github.com/yourusername/yourrepository.git
```

#### 4) 파일 업로드
```sh
git push -u origin master
```

---
이 문서를 지속적으로 업데이트하며 유용한 Linux 명령어들을 정리할 수 있습니다! 🚀

