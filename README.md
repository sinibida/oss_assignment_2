# 5월 12일 과제 조사 내용 (by. 01분반 20223157 장준하)

(어딘가(?)에 가로줄 사용하기)
(볼드체, 이탤릭체 적극 활용할것!)

## Linux 명령어

(표로 명령어 요약하기)

### 1. top

(사용 예시를 소스코드로 표시)

### 2. ps

(사용 예시를 소스코드로 표시)

### 3. jobs

(사용 예시를 소스코드로 표시)

### 4. kill

(사용 예시를 소스코드로 표시)

## vim 에디터 속 매크로 기능

### 1. 매크로란?

[**매크로**](https://ko.wikipedia.org/wiki/%EB%A7%A4%ED%81%AC%EB%A1%9C_(%EC%BB%B4%ED%93%A8%ED%84%B0_%EA%B3%BC%ED%95%99) "관련 위키피디아 링크")란 여러 입력이 어떤 여러 출력으로 변환되야 하는지 알려주는 규칙이다. 주로 여러 입력을 짧게 단축하기 위해 사용된다.
프로그래머는 이 기능을 이용해 반복적이고 번거로운 편집 작업을 더 쉽고 안정성 있게 수행할 수 있다.

여러 텍스트 에디터에서 매크로를 지원하는데, vim 에디터에서도 이 기능을 사용할 수 있다. 

### 2. 매크로 녹화법

vim에서 매크로를 사용하려면 먼저 매크로를 레지스터*register*에 녹화해야 한다.

1) `q<레지스터 이름>`를 입력해 녹화를 시작 한다. 주로 레지스터 이름은 소문자 한개이다.
2) 녹화할 커맨드를 입력한다.
3) 다시 `q`를 눌러 녹화를 중지한다.

#### 예시

`qaiabc<Esc>q`

+ `qa` : 'a' 레지스터에 녹화 시작.
+ `iabc<Esc>` : *입력모드에서 `abc` 입력 후 입력모드 퇴장.* (녹화되는 커맨드)
+ `q` : 녹화 중지

### 3. 매크로 사용법

### 4. 녹화해놓으면 유용한 매크로

(매크로들을 불렛으로 요약)

(매크로를 사용하는 모습을 gif로 올리기)
