# 설계

## 용어

### 사용자

> 로그인이 가능한 사용자를 의미한다

> 지정된 권한을 사용자에게 직접 부여하거나

> 소속된 그룹에 부여된 권한에 따라 시스템을 사용 가능하다

### 그룹

> 권한을 갖는 대상으로 사용자를 포함시켜 사용자에게 권한을 부여할 수 있다

> 하나의 사용자는 복수의 그룹에 포함 될 수 있다

### 부서

> 하나의 사용자는 하나의 부서에 편입 될 수 있다

> 어떤 작업에 대한 목표 대상으로써 사용되게 되며 그룹과 달리 권한을 갖지 않는다

### 권한

> 프로그램 개발시 정적으로 만들어지며 사용자는 부여된 권한에 따라 기능이 제한된다

---

### 회사

> 거래(구매/판매/외주)하게 되는 대상 회사를 의미 한다

---

### 프로젝트

> 고객회사와의 작업의 기준이 되며 고객 담당자의 정보를 갖습니다

> 구매와 판매의 기준이 되어 프로젝트 진행중 발생한 비용과 수익에 대한 분석의 기준이 됩니다

---

### 공정 분류

> 공정의 처리방식과 필요정보가 동일한 그룹화의 큰 단위

> 예) 인쇄, 톰슨, 포장, 성형, 코팅

### 공정 유형

> 공정 분류에서 좀더 구체화되는 개념

> 기준 단가와 난이도별 비율을 통해 단가를 산출의 기준이 된다

> 공정에서 차지하는 노무비(직접/간접), 간접 재료비, 간접 경비의 비율을 관리하여 단가 산정의 기준으로 사용한다

### 공정

> 품목과 1:1 로 매칭되는 제조 과정을 의미한다

> 공정 유형과 난이도를 지정하여 공정 단가가 책정된다

> 공정에 대한 상세한 설명가 부가정보(문서/사진 등)가 저장된다

---

### 품목 분류

> 품목을 계층형으로 분류하는 단위가 된다

> 분류의 단위는 이후 다양한 분석의 기준이 된다

### 품목

> 취급(판매/생산/구매)되는 모든 품목을 의미

### 품목 스펙

> 품목을 구매시 입력하는 정보에 따라 단가가 변동되는 방식을 의미한다

> ex) 용지의 정보(넓이/높이/절수)에 따라 단가가 변동

---

### 견적

> 프로젝트를 지정하여 프로젝트의 고객 담당자에게 견적을 작성한다

> 견적 대상 품목은 기존에 존재하지 않기 때문에 품목과 BOM을 바로 생성하여 작성 가능하다


```

![입고흐름](/design/흐름.puml)

### 자재확보 - 구매자재

![자재확보-구매자재](/design/자재확보-구매자재.puml)

### 자재확보 - 생산자재

![자재확보-생산자재](/design/자재확보-생산자재.puml)

### 자재확보 - 외주자재

![자재확보-외주자재](/design/자재확보-외주자재.puml)

```

