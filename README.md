# 5월 12일 과제 조사 내용 (by. 01분반 20223157 장준하)

(어딘가(?)에 가로줄 사용하기)
(볼드체, 이탤릭체 적극 활용할것!)

## Linux 명령어

|top|ps|jobs|kill|
|---|--|----|----|
|   |

(표로 명령어 요약하기)

### 1. top

![top 사용법](/images/linux/top.gif?raw=true)

현재 리눅스 시스템의 상태 및 현재 실행 중인 프로세스 목록을 보여주는 명령어이다.
종료될 때까지 지속적으로 새로고침 되며, 실행 중 커맨드를 사용할 수 있다.

#### 사용법

`top -b -d secs -n max`

+ -b : batch 모드로 실행
+ -d secs : 새로고침 주기 (초)
+ -n max : 새로고침 횟수

명령어를 실행한 뒤 `q`를 눌러 *top* 명령어를 중지하고 `k` 명령어로 실행중인 프로그램을 종료할 수 있다.

### 2. ps

![ps 사용법](/images/linux/ps.gif?raw=true)

현재 실행 중인 프로세스 목록을 보여주는 명령어이다.

#### 사용법

`ps -efl`

+ -e : 모든 프로세스 표시
+ -f, -l : 프로세스 추가정보 표시 (실행한 유저, ppid, etc.)

### 3. jobs

(TODO 이미지 추가)

현재 쉘 안에서 실행중인 프로세스 목록을 보여주는 명령어이다.
*kill* 또는 *fg* 명령어에서 사용할 수 있는 job number를 제공한다.

#### 사용법

`jobs -lrs`

+ -l : Process ID 표시
+ -r : 실행중인 프로세스만 표시
+ -s : 정지된 프로세스만 표시

### 4. kill

(TODO 이미지 추가)

실행 중인 프로세스에게 종료 신호를 보내는 명령어이다.

#### 사용법

`kill -sigspec %jobnumber`

+ -sigspec : - 뒤에 종료 신호 입력 (아래 설명 참조) 
+ %jobnumber : *jobs* 명령어로 구할 수 있는 job number 입력

#### 종료 신호

+ 6 (SIGKILL) : 강제 종료, 종료되는 프로세스가 이를 취소할 수 없다.
+ 15 (SIGTERM) : 종료 요청, 종료되는 프로세스가 이를 받고 취소하거나 종료 준비를 할 수 있다.

## vim 에디터 속 매크로 기능

### 1. 매크로란?

(매크로에 대한 위키피디아 주소로 링크 만들기)

### 2. 매크로 녹화법

### 3. 매크로 사용법

### 4. 녹화해놓으면 유용한 매크로

(매크로들을 불렛으로 요약)

(매크로를 사용하는 모습을 gif로 올리기)

