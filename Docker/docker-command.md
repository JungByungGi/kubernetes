도커 명령어 사용하기
====================

* 도커 명령어로 검색
```
docker search nginx
```

* 도커 이미지 다운로드
```
docker pull nginx
```

* 도커 이미지 정보 확인
```
docker inspect nginx
```

* 도커 이미지 확인
```
docker images
```

* 도커 이미지 삭제
```
docker rmi nginx
```

* 도커 컨테이너 생성
```
docker run -d --name nx nginx
```

* 실행 중인 컨테이너 확인
```
docker ps
```

* 모든 컨테이너 확인
```
docker ps -a
```

* 컨테이너 중지
```
docker stop {container_id}
```

* 컨테이너 삭제
```
docker rm {container_id}
```

* 포트포워딩으로 톰캣 실행
```
docker run -d --name tc -p 80:8080 tomcat
```

* 컨테이너 내부 쉘 실행
```
docker exec -it tc /bin/bash
```

* 컨테이너 로그 확인
```
docker logs tc
```

* 호스트 및 컨테이너 간 파일 복사
```
docker cp <path> <to container>:<path>
docker cp <from container>:<path> <path>
docker cp <from container>:<path> <to container>:<path>
```

* 임시 컨테이너 생성
```
docker run -d -p 80:8080 --rm --name tc tomcat
```




