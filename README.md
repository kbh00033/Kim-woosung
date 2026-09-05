#프로젝트명
개인 프로필 사이트 만들기

##프로젝트에 대한 간단한 설명
AI로 기본 틀을 잡은 다음 추가로 제가 속한 동아리에 대해 소개하는 콘텐츠를 담았다

Vercel Deploy URL: https://kim-woosung-6gp4.vercel.app
index.html URL: https://kim-woosung-6gp4.vercel.app/index.htmlindex2.html 
URL: https://kim-woosung-6gp4.vercel.app/index2.html

###Key Learning
1. Git이란 버전관리를 편리하게 하는 프로그램이며 VS code에 Git를 연동하는 방법에 관하여 배웠다.
2. VS Code에서 작성한 파일을 Git에 Commit하고 Push하는 명령어 및 방법에 관해 배웠다
3. 실제로 누구나 사이트에 접속할 수 있도록 Vercel에 배포하는 법에 관하여 배웠다

####Development Flow
0. git clone (repo URL) 명령어를 VS Code 터미널에 입력해 프로젝트 시작 전 원하는 로컬 폴더 안에 연동합니다
1. VS Code에서 파일을 작성하고 Command+S로 저장합니다
2. VS Code에서 Git repository와 연동이 완료되었다는 하에 해당 Git repository에 commit합니다
(이때 git commit -m “수정사항” 명령어를 입력합니다)
3. git push (mine<-자신이 선택한 repository 별명) main 명령어로 Push(업로드)합니다
4. Vercel에 로그인 후 Add New를 클릭하여 자신이 업로드한 Git을 선택한 후 배포합니다

#####Code Modification
제가 다니는 한동대학교에 대해 소개하는 위키백과와 위치를 안내하는 구글지도 하이퍼링크를 추가하였습니다
제가 속한 동아리인 HAC에 대해 소개하는 글과 이미지를 탑재하였습니다
제 프로필 사진을 파란 하늘로 업데이트 하였습니다
HTML 문법 상 오류(<img src=”~” arc(->art)=“~” >및 <ul> ~ </ul>안에 <p> ~ </p>를 작성한 오류를 수정하였습니다

######Problem & Solution
commit의 수정사항에 오타가 생겼을 경우
git commit --amend -m “수정사항”을 입력한다
git push (mine<-자신이 선택한 repository 별명) main --force로 강제 업로드를 실시한다

새로운 파일이 0byte가 아님에도 불구하고 git에 0byte로 Push된 경우
git add (파일명 혹은 .) 입력한다
git commit --amend -m “수정사항”을 입력한다
git push (mine<-자신이 선택한 repository 별명) main --force로 강제 업로드를 실시한다

#######Reflection
img파일을 로컬폴더에서 연결할 경우 다른 기기의 웹사이트에서 들어갈 경우 표시되지 않는다는 것을 알게 되었다
유튜브 영상이나 동영상을 임베디드 하는 법이 궁금하다