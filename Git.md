# Git 정리

## Git의 기본

### Git 이란?

소스코드를 효과적으로 관리하기 위해 개발된 **분산형 버전 관리 시스템**

### 이력을 관리하는 저장소

- 저장소(repository); 파일이나 폴더를 저장해 두는 곳

- Git이 제공하는 저장소: 원격저장소(Remote Repository)&로컬저장소

![image](https://backlog.com/git-tutorial/kr/img/post/intro/capture_intro1_2_2.png)

### 커밋(Commit)

- 파일 및 폴더의 추가/변경 사항을 저장소에 기록하기 위한 명령어

### Work tree & Index

```
work tree=working directory

index=staging area
```

![image2](https://backlog.com/git-tutorial/kr/img/post/intro/capture_intro1_4_1.png)
```
등록=add
```

## Commit

- 흐름
    
    1. 작업을 하고
    2. 변경된 파일을 모아(add)
    3. 버전으로 남긴다(commit)

- 명령어
    1. **git init**; 새로운 저장소 생성
    2. **git add <file/directory>**; work tree 상의 변경 내용을 Index 영역에 추가
    3. **git commit -m '메시지'**; 커밋
    4. git status; working directory와 staging area 상태 확인
    5. git log; commit된 파일 파악

## 저장소 공유하기

### push

; 로컬 저장소에서 변경된 이력을 원격 저장소에 공유하기 위해 로컬 저장소의 변경 이력을 원격 저장소에 업로드하는 명령어

### clone

; 원격 저장소 복제하는 명령어

```
이를 통해 복제한 저장소를 다른 PC에서 로컬 저장소로 사용할 수 있다.
```

### pull

; 원격 저장소에서 로컬 저장소로 업데이트 하기위한 명령어

## 변경 이력 병합하기

### merge

; 각 branch에서 작업을 한 이후 이력을 합치기 위해 사용하는 명령어