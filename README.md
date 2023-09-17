주요 명령어

minikube multi node 실행

```
minikube start --nodes 3 --driver-docker
```

docker 드라이버로 minikube 실행시 외부 포트 접속 하려면 아래와 같이 해야함

```
// svc 목록 확인
minikube service list
// 외부 포트 접속
minikube service
```

## minikube 노드 이름 규칙 (kubernetes.io/hostname)

minikube, minikube-m02, minikube-m03, ...
