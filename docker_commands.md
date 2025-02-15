
#### 다음 명령어를 실행하여 컨테이너를 빌드하고 실행합니다.

```sh
docker-compose up -d
```

#### 컨테이너 내부로 접속하여 bash 를 실행하던지 python 을 실행하던지(둘중의 하나)
```sh
docker exec -it python-dev bash
docker exec -it python-dev python
```

### 컨테이너 관리

#### 컨테이너 정지
```sh
docker-compose down
```

#### 컨네이너 삭제 및 초기화
```sh
docker-compose down --volumes
```

####  docker-compose up -d 는 기존 이미지를 사용하며, Dockerfile이 변경되어도 자동으로 새로운 이미지를 만들지 않음

####  Dockerfile 이나 requirements.txt 를 수정했을 경우 반드시 docker-compose build를 실행해야 반영됨

#### 만약 매번 빌드하고 싶다면 docker-compose up -d --build 를 사용할 수도 있지만, 불필요한 재빌드를 하지 않으려면 docker-compose build 를 명시적으로 따로 사용하는 것이 좋다.


