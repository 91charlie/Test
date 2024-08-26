# Git 명령어 정리       
## git 저장과정 - LR 생성 => WD => (add) => SA => (commit) => LR    
## 매 과정 사이에 "git status" 명령어를 통해 상태를 확인한다.

1. git init   
pc에 새로운 git 저장소 (LR(local repository))를 생성할 때 사용되는 명령어

    >이 명령어를 통해 git 폴더(LR(Local Repository)) 생성 후 기록 가능   
    >개인의 작업폴더가 .git으로 기록 가능한 폴더로 만들어진다.
   
   <br><br>

2. git add "" <= ""는 파일 "이름.확장자"를 의미한다. 예) git add filename.txt   

    >Working directory (작업 구간)에서 추가되거나 수정된 내용을 Staging area(대기공간)으로 추가시킬 경우에 사용하는 명령어 WD의 파일이 SA에 추가되면서 Untracked => Tracked 상태로 바뀐다.

    >이미 SA(Staging Area)에 add된 파일일 경우에도 WD(Working Directory)에서 추가되거나 수정된 내용이 있을 경우 add를 다시해주어야 SA에 적용된다.

<br><br>

3. git commit -m "Labeling 내용" <= ""안에 커밋 메세지를 입력한다. 이는 커밋이라는 박스의 라벨 역할을 한다.   
    WD에서 SA에 추가된 파일들을 LR에 기록하는 명령어   
   
    >Staging Area에서 Commit대기 중인 파일들을 "커밋 메세지"와 함께 하나로 commit 하여 LR에 저장하게 된다.   
      
    >파일들이 commit되어 LR에 저장되면 SA는 비어있는 상태가 된다. 

    >따라서 git add 명령어를 사용하여 같은 버전으로 작업된 파일들을 SA에 추가시킨뒤 commit-m- "" 명령어를 사용하여 커밋메세지와 하나로 LR에 저장 후 다른 버전의 파일또한 
       
        WD(add) => SA => (commit) => LR 과정을 통해 각각 다른버전으로 저장할 수 있다.   
        

