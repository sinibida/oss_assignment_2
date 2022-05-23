# 5월 12일 과제 조사 내용 (by. 01분반 20223157 장준하)

## Linux 명령어

이 과제에선 쉘 내에서 실행 중인 프로세스들을 관리하는데 유용한 **top, ps, jobs, kill 명령어**에 대해 조사하였다.

|명령어|설명|
|---|---|
|**top<br>ps<Br>jobs**|실행 중인 프로세스 목록 조회|
|**kill**|실행 중인 프로세스 종료|

---

### 1. top

![top 사용법](/images/linux/top.gif?raw=true)

현재 리눅스 시스템의 상태 및 현재 실행 중인 프로세스 목록을 보여주는 명령어이다.
종료될 때까지 지속해서 새로고침 되며, 실행 중 커맨드를 사용할 수 있다.

#### 사용법

`top -b -d secs -n max`

+ **-b** : batch 모드로 실행
+ **-d secs** : 새로고침 주기 (초)
+ **-n max** : 새로고침 횟수

명령어를 실행한 뒤 `q`를 눌러 *top* 명령어를 중지하고 `k` 명령어로 실행 중인 프로그램을 종료할 수 있다.

---

### 2. ps

![ps 사용법](/images/linux/ps.gif?raw=true)

현재 실행 중인 프로세스 목록을 보여주는 명령어이다.

#### 사용법

`ps -efl`

+ **-e** : 모든 프로세스 표시
+ **-f, -l** : 프로세스 추가정보 표시 (실행한 유저, ppid, etc.)---### 3. jobs

![jobs 사용법](/images/linux/jobs.gif?raw=true)

현재 쉘 안에서 실행 중인 프로세스 목록을 보여주는 명령어이다.
*kill* 또는 *fg* 명령어에서 사용할 수 있는 job number를 제공한다.

#### 사용법

`jobs -lrs`

+ **-l** : Process ID 표시
+ **-r** : 실행 중인 프로세스만 표시
+ **-s** : 정지된 프로세스만 표시

---

### 4. kill

![kill 사용법](/images/linux/kill.gif?raw=true)

실행 중인 프로세스에 종료 신호를 보내는 명령어이다.

#### 사용법

`kill -sigspec %jobnumber`

+ -**sigspec** : - 뒤에 종료 신호 입력 (아래 설명 참조)
+ %**jobnumber** : *jobs* 명령어로 구할 수 있는 job number 입력
