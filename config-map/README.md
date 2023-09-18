## Secret

Key: value

PW: Base64로 변환해서 입력해야함

Pod에 주입될때 자동으로 Decoding됨

값이 메모리에 저장됨 .

1Mbyte까지 저장 가능

file로 만들때는 내용이 자동으로 base64로 인코딩됨

## literal, file, volume mount

```
// config map 생성
kubectl create configmap cm-file --from-file=./config-map/file-c.txt
// secret 생성
kubectl create secret generic sec-file --from-file=./config-map/file-s.txt
```

pod 생성 후 config map을 변경하면 다른 결과가 나타난다.

- literal: 변화없음 (pod을 다시 생성해야 반영됨)
- file: 변화없음 (pod을 다시 생성해야 반영됨)
- volume mount:
