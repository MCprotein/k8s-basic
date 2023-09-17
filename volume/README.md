## emptyDir

컨테이너 공유 마운트 볼륨. Pod과 생명주기 같음

## hostPath

각 노드의 Path 사용. Pod과 관련 없음

다만 Pod이 다른 노드에 새로 생성될때는 기존 볼륨에 마운트 할 수 없음

사전에 hostPath가 미리 생성되어있어야함.

노드의 데이터를 Pod에서 쓰기 위한 목적

## PVC/ PV

영속성 볼륨

K8S는 User와 Admin의 영역이 분리되어 있음

PV는 어드민이 생성

사용자가 PVC 생성

Pod에는 PVC와 연결
