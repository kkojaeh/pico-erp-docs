# 설계

## 흐름

![입고흐름](/design/흐름.puml)

```

![입고흐름](/design/흐름.puml)

### 자재확보 - 구매자재

![자재확보-구매자재](/design/자재확보-구매자재.puml)

### 자재확보 - 생산자재

![자재확보-생산자재](/design/자재확보-생산자재.puml)

### 자재확보 - 외주자재

![자재확보-외주자재](/design/자재확보-외주자재.puml)

```

```memaid
sequenceDiagram
    participant Alice
    participant Bob
    Alice->John: Hello John, how are you?
    loop Healthcheck
        John->John: Fight against hypochondria
    end
    Note right of John: Rational thoughts <br/>prevail...
    John-->Alice: Great!
    John->Bob: How about you?
    Bob-->John: Jolly good!
```
