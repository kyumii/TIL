# GitHub 특강 Day 1

## 1. 버전관리

- __용어__
  - 버전 : 컴퓨터 소프트웨어의 특정 상태
  - 관리 : 어떤 일의 사무, 시설이나 물건의 유지,계량
  - 프로그램 : 컴퓨터에서 실행할때 특정 작업을 수행하는 일련의 명령어들의 모음
- __Git__ 
  - 버전 관리 프로그램 
  - 백업, 복구, 협업



## 2. CLI / GUI

- __CLI__
  - Command Line Interface
  - 터미널을 통해 사용자와 컴퓨터가 상호작용하는 방식
  - 단계가 적고, 컴퓨터의 성능을 더 적게 소모
  - GUI로는 불가능한, 많은 세부적인 기능 사용가능



- __GUI__
  - Graphic User Interface
  - 그래픽을 통해 사용자와 컴퓨터가 상호작용하는 방식
  - 많은 사람들이 더 쉽게 컴퓨터 사용 가능
  - PC 대중화의 주요 요인



- _Interface (인터페이스)_
  - _서로 다른 개체끼리 맞닿아 있는 면_
  - _사용자와 컴퓨터가 서로 소통하는 접점_



- git bash
  - 명령어 통일하기 위함
    - UNIX, Windows 명령어의 차이
    - UNIX계열 운영체제 명령어를 더 많이 씀
      - _개발자 입장_



## 3. 경로

- 루트 디렉토리 
  - Root Directory, /
  - 모든 파일과 폴더를 담고있는 최상위 폴더
- 홈 디렉토리
  - Home Directory, ~
  - Tilde(틸드)라고도 부름
  - 현재 로그인 된 사용자의 홈 폴더 
- 절대 경로
  - 루트 디렉토리부터 목적 지점까지 거치는 모든 경로를 전부 작성한 것
- 상대 경로
  - 현재 작업하고 있는 디렉토리를 기준으로 계산된 상대적 위치를 작성한 것
  - `./` : 현재 작업하고 있는 폴더를 의미
  - `../` : 현재 작업하고 있는 폴더의 부모 폴더를 의미

## 4. 터미널 명령어

- `touch`

  - 파일을 생성하는 명령어
  - 띄어쓰기로 구분하여 여러 파일을 한꺼번에 생성 가능
  - 숨김 파일을 만들기 위해서는 .을 파일 명 앞에 붙임

- `mkdir`

  - make directory
  - 새 폴더를 생성하는 명령어
  - 띄어쓰기로 구분하여 여러 파일을 한꺼번에 생성 가능
  - 띄어쓰기로 구분하여 여러 파일을 한꺼번에 생성 가능

- `ls`

  - list segments
  - 현재 작업 중인 디렉토리의 폴더/파일 목록을 보여주는 명령어
  - `-a` : all 옵션. 숨김 파일까지 모두 보여줌
  - `-l` : long 옵션. 용량, 수정 날짜 등 파일 정보를 자세히 보여줌

- `mv`

  - move
  - 폴더/파일을 다른 폴더 내로 이동 하거나 이름을 변경하는 명령어
    - 단, 다른 폴더로 이동할 때는 작성한 폴더가 반드시 있어야 합니다. 
    - 없으면 이름이 바뀝니다.

- `cd`

  - change directory
  - 현재 작업 중인 디렉토리를 변경하는 명령어
  - `cd ~` 를 입력하면 홈 디렉토리로 이동합니다. (단순히 `cd` 라고만 입력해도 동일합니다.)
  - `cd ..` 를 입력하면 부모 디렉토리로 이동합니다. (위로 가기)
  - `cd -` 를 입력하면 바로 전 디렉토리로 이동합니다. (뒤로 가기)

- `rm`

  - remove
  - 폴더/파일 지우는 명령어
  - GUI와 달리 휴지통으로 이동하지 않고, 바로 `완전 삭제`합니다.
  - `*(asterisk, wildcard)`를 사용해서 `rm *.txt` 라고 입력하면 txt 파일 전체를 다 지웁니다.
  - `-r` : recursive 옵션. 폴더를 지울 때 사용합니다.

- `start, open`

  - 폴더/파일을 여는 명령어
  - `Windows`에서는 start를, `Mac`에서는 open을 사용할 수 있습니다.

  

  

- __유용한 단축키__

  - `위, 아래 방향키` : 과거에 작성했던 명령어 조회

  - `tab` : 폴더/파일 이름 자동 완성

  - `ctrl + a` : 커서가 맨 앞으로 이동

  - `ctrl + e` : 커서가 맨 뒤로 이동

  - `ctrl + w` : 커서가 앞 단어를 삭제

  - `ctrl + l` : 터미널 화면을 깨끗하게 청소 (스크롤 올리면 과거 내역 조회 가능)

  - `ctrl + insert` : 복사

  - `shift + insert` : 붙여넣기



- 수업 시간에 한 명령어

```bash
 # 폴더 생성
 mkdir CLI
 mkdir 'multi campus'

 # 목록 조회
 ls
 ls -a
 ls -l
 ls -a -l

 # 위치 변경
 cd CLI
 cd ..
 cd ~

 # 파일 생성
 touch a.txt
 touch a.txt b.txt c.txt

 # 파일, 폴더 제거
 rm a.txt
 rm -r new

```





## 5. 마크다운

1. 장점
   - 문법이 직관적이고 쉽습니다.
   - 관리가 쉽습니다.
   - 지원 가능한 플랫폼과 프로그램이 다양합니다.
2. 단점
   - 표준이 없어 사용자마다 문법이 상이할 수 있습니다.
   - 모든 HTML 마크업 기능을 대신하지는 못합니다.
3. 주의사항
   - 마크다운의 본질은 글에게 `역할`을 부여하는 것입니다.
   - 따라서 반드시 `역할`에 맞는 마크다운 문법으로만 작성해야 합니다.
   - 예를 들면 `글씨의 크기를 키우고 싶다`는 이유로 `내용`에게 `제목`의 역할을 부여하면 안됩니다. (이 부분은 마크다운 문법을 학습하면서 자연스럽게 이해할 수 있습니다.)

- 문법

1. 제목

# 	제목 1

## 	제목2

### 	제목 3

#### 	제목4

##### 	제목5

###### 	제목6

___



2. 목록

   __순서가 없는 목록__

- 과일
  - 사과
  - 바나나

​	__순서가 있는 목록__

1. 목록1
2. 목록2
   1. 목록2-1
   2. 목록2-2

----

강조(스타일링)

1. 기울임(이텔릭체) :*글자*, _글자_
2. 굴게 볼드체 : **글자**, __글자__
3. 취소선 : ~~글자~~

---

코드

인라인 코드(=한줄) -> 백틱(backtick) `

파이썬에서는 `print("Hello world!")` 라고 쓸 수 있습니다.



블록 코드(=여러줄)

```python
for i in range(10):
    print(i)
```



표(table)

| 사자 | 호랑이 |
| ---- | ------ |
|      |        |

| --   | --   | --   |
| ---- | ---- | ---- |
|      |      |      |
|      |      |      |
|      |      |      |



'print'\

