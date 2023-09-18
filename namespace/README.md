## ResourceQuota

Namespace마다 자원의 최대량을 제한

## LimitRange

Namespace에 들어오는 Pod의 크기를 제한

ResourceQuota와 LimitRange는 Cluster자체에도 설정 가능

## Namespace

Node, PV등과 같이 모든 노드에서 사용되는 자원이 아니라면, Namespace별로 자원이 구분된다.
통신도 불가
오브젝트끼리의 연결은 같은 Namespace끼리만 가능
