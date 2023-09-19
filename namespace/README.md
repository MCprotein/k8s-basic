## ResourceQuota

Namespace마다 자원의 최대량을 제한

## LimitRange

Namespace에 들어오는 Pod의 크기를 제한

ResourceQuota와 LimitRange는 Cluster자체에도 설정 가능

## Namespace

Node, PV등과 같이 모든 노드에서 사용되는 자원이 아니라면, Namespace별로 자원이 구분된다.
통신도 불가
오브젝트끼리의 연결은 같은 Namespace끼리만 가능

host-path는 namespace와 무관하게 사용이 된다. 이것을 방지하려면 pod의 user의 권한을 root가 아니라 다른 것으로 해야한다.
