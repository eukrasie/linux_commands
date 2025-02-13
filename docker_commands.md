#### 다음 명령어를 실행하여 컨테이너를 빌드하고 실행합니다.

'''sh
docker-compose up -d
'''

#### 컨테이너 내부로 접속하여 bash 를 실행하던지 python 을 실행하던지(둘중의 하나)
'''sh
docker exec -it python-dev bash
docker exec -it python-dev python
'''

### 컨테이너 관리

#### 컨테이너 정지
'''sh
docker-compose down
'''

#### 컨네이너 삭제 및 초기화
'''sh
docker-compose down --volumes
'''


