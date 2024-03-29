**Writing on Github**

2018-09-06
Jun Sok Huhh | :house:[lostineconomics.com](https://anarinsk.github.io/)



# Github 

한마디로 축복이다. 이런 서비스가 세상에 있다니! 문돌이로서 git과 github(깃헙)를 처음 접했을 때는 솔직히 당황스러웠다. 그저 드롭박스, 에버노트 정도의 서비스만 이해할 수 있었던 나에게 version control system(VCS)라는 건 크게 와닿지 않았다. 하지만 필요는 발명의 어머니. 허접하지만 코드 관리와 프로젝트 관리가 필요해지면서 어쩔 수 없이 쓰게 되었고, 이제는 그나마  많이 익숙해졌다.(라고 하기에는 git의 너무나 많은 훌륭한 기능 중에서 대략 5% 정도 쓰고 있는 듯... ㅠㅠ) 

깃헙은 git이라는 VCS의 원격 저장소를 웹으로 뽑아낸 서비스다. 보통 개인 혹은 회사가 git을 구축하면 로컬 머신들이 접속하는 서버를 필요로 한다. 이걸 별도의 웹 서비스로 제공한다고 생각하면 대충 맞을 것이다. 그런데, 깃헙은 말 그대로 git의 허브 이상의 쓰임새를 제공한다. 뒤에서 다시 다루겠지만, 조금만 살펴보면 깃헙 자체를 꽤 유용한 웹하드 그리고 블로그 호스팅 서비스로도 활용할 수 있다. 

# Markdown 

마크다운(md)은 워드 프로세서와 같은 WYSIWYG의 장점을 잃지 않으면서 최소한의 마크업을 통해서 문서의 표현력까지 높이는 문서화 도구다. 한마디로 워드처럼 내용을 타이핑하면서도 여러가지 문서 표현(장, 절 제목 구분, 이미지 넣기, 태그 넣기, 수식) 등을 간단한 마크업으로 해결하겠다는 것이 이 언어의 목표다. 지금까지 써본 경험으로 말하자면 마크다운은 상상했던 것보다 훨씬 편하고 좋다. 학습곡선도 그리 가파르지 않다. 솔직히 학습 곡선에서는 html이나 $\LaTeX$에 비할 바가 아니다. 

## html &harr; md 

html과 md 사이는 쉽게 오갈 수 있다. 웹 문서로 쉽게 바꿀 수 있다는 것은 소통에 있어 엄청난 장점 아닐까? $\LaTeX$으로 소통할 때의 무거움과 답답함을 떠올려 보자. 

## Almost WYSIWYG  

마크업 언어의 문제는 결과를 바로 바로 보기 어렵다는 것이다. $\LaTeX$이 극단적인 사례 중 하나일 것이다. 써보신 분들은 알겠지만, 아름답고 유려한 문서를 얻는 대신 $\LaTeX$을 컴파일 하는 데에는 상당한 시간과 노력이 든다. 솔직히 이 점에서 생산성에 도움이 되는 도구인지는 의문이다. 그보다는 과학자를 위한 미적 도구라고 부르는게 맞을 듯 싶다.

## No installation!

설치형 md 에디터가 시중에 몇 개 있긴 하지만 필수는 아니다. 깃헙만 해도 그냥 웹에서 마크다운 문법으로 적은 후 commit(실행)하면 화면에 척 붙는다. 지금 이 글을 작성하는 것도 웹 기반으로 돌아가는 stackedit이다. 설치가 필요 없고 웹에서고 가볍게 돌기 때문에 모바일, 태블릿 환경에서 쓰기에는 모자람이 없다. 

# My Case 

내가 현재 쓰고 있는 문서화 작업 흐름을 간략하게 소개하겠다. 그냥 이렇게도 쓸 수 있구나, 정도로 봐주시면 되겠다. 

## Documentation 

앞서 언급했던 (PC든 모바일이든) [stackedit.io](https://stackedit.io/app#)를 띄운 후 외부 저장소의 작업 환경을 불러 온다. 오른쪽에 싱크 옵션을 누르면 동기화를 실현할 수 있는 옵션이 세 개 뜬다. 클릭 후 각자 특성에 맞게 로긴을 해주면 되겠다. 한번만 해주면 된다. 
    ![](http://raw.githubusercontent.com/anarinsk/public_writing/master/workflow_with_github/assets/images/workflow_1.png)

![](http://raw.githubusercontent.com/anarinsk/public_writing/master/workflow_with_github/assets/images/workflow_2.png)

이중에서 메인으로 쓸 저장소를 하나 지정한다. 이 녀석은 기본적인 환경과 임시 문서 따위를 저장, 관리한다. 저장 옵션에 반갑게도 깃헙이 있다. 이렇게 외부 계정과 stackedit을 연동하면 끝이다. 메인 저장소에서 작업 환경을 불러와서 이를 로컬 머신에서 그대로 재현해준다. 이렇게 재현된 환경은 브라우저 화면 왼쪽에서 확인할 수 있다. 어떤 소프트웨어의 설치도 별도의 서비스 가입도 필요 없다. 

![](https://raw.githubusercontent.com/anarinsk/public_writing/master/workflow_with_github/assets/images/workflow_3.PNG)

stackedit은 소스를 깃허브에서 읽은 후 이를 브라우저에 올리는 방식으로 구현된다. 따라서 소스가 브라우저로 로딩 되는 짧은 시간 이외에는 별도로 필요한 것이 없다. 쉽게 말해 클라우드 작업 환경을 쉽게 구축할 수 있다. 

## May the Github with you 

기본적인 환경을 저장하는 데에는 google drive도 나쁘지 않다. 하지만 이외 개별 문서를 저장하는 데에는 깃헙을 활용하는 편이 낫다. 깃헙은 달에 8달러씩 내면 pivate 계정을 가질 수 있고, 무료로 쓰면 public으로만 쓸 수 있다. 8달러를 들이는 게 아깝다면, 비공개 문서는 google drive에 두고 공유하고 싶은 문서만 깃헙으로 보내면 된다. 공유라는 면에서는 google drive보다 깃헙이 압도적으로 편하고 바람직하다. 아울러 깃헙 리포지터리의 대문 역할을 하는 `README.md` 파일들도 쭉 끌어다 stackedit에 두면 add-commit-push 사이클 없이 수시고 고치며 내용을 다듬을 수 있다. 

## Simplest blog ever

관리와 홍보 등의 목적을 위해서 라면 큰 회사들이 서비스하는 블로그를 쓰거나 아니면 별도의 호스팅 서비스를 통해 wordpress 같은 전문툴을 깔아 쓰는게 필요하다. 물론 여기에는 치러야 하는 비용도 있다. 전자는 나중에 내용을 백업하거나 이전할 때 몹시 불편하다. 네이버 블로그만 해도 데이터베이스 백업을 지원하지 않는다. 독립성이나 잔재미라는 면에서 워드프레스 같은 툴을 호스팅 서비스에 직접 깔아 쓰면 좋지만, 어쩔 수 없는 관리의 이슈가 있다. 보안 상의 이슈 등으로 기반 서비스를 종종 업데이트해야 하는 데 사실 귀찮다.  

문득 이런 생각이 들었다. 어차피 요즘 같은 소셜의 시대에 내 글에 와서 굳이 그 위에 댓글을 달라고 해야 할까? 차라리 글을 어디 던져 놓고 피드백은 소셜미디어로 주고 받으면 되지 않나? 잡스러운 것 없이 그냥 글만 깔끔하게 전달할 수 있으면 좋겠는데... 

사실 깃헙 위에서도 상용 블로그 못지 않은 서비스를 운용할 수 있다. [jekyll](https://jekyllrb.com/)이나 [Hugo](https://gohugo.io/)를 이용하면 된다.  깃헙에 이런 전문형 블로그 만드는 방법은 구글링을 해보시면 많이 나오니 굳이 여기서 반복하지는 않겠다. 

하지만 더 미니멀한 목적을 추구하는 나에게는 이것도 꽤 부담스러웠다. 포스트의 링크를 보여줄 수 있는 대문 페이지가 있으면 족했다.

이런 생각으로 만든 것이 [lostineconomics.com](https://anarinsk.github.io)다. 보시면 약간의 설명과 이미지 그리고 글들의 링크 밖에 없다. 이 페이지는 anarinsk.github.io 깃헙 리포지토리의 index.md  파일을 수정하는 것으로 손쉽게 구현된다. 얼마나 간편한가? 페이지의 포스트는 내 깃헙의 여러 리다른포지터리에 있다. 

### For html link in github 
깃헙 안에 위치하는 html 문서들은 렌더링이 되지 않고 소스 그대로 노출된다. 따라서 html 링크를 걸고 이를 렌더링하고 싶다면 다른 서비스를 하나 거치면 된다.  두 개의 서비스를 추천한다. 

[rawgit.com](https://rawgit.com)
[htmlpreview](https://htmlpreview.github.io)

# Miscellaneous 

## What about math? 

md가 $\LaTeX$을 본격적으로 대체할 수는 없다. 하지만 수식은 인라인(글 내부)든 디스플레이 모드이든 제약 없이 쓸 수 있다. $\alpha$ 솔루션은 아닐지 모르지만 $\beta$나 $\gamma$ 정도로는 부족함이 없어 보인다. 

$$
U = u(x,y) ~ \text{s.t.}~p_x x + p_y y \leq m
$$

이 정도면 뭐 아쉬운 대로 쓰기 충분하지 않은가? 

## What about collaboration? 

git은 VCS다. 따라서 협업 대상이 뭔가 수정을 하면 기록이 자동으로 남고 그걸 언제든 조회할 수 있다. 깃허브 홈페이지 들어가면 누가 뭘 어떻게 고쳤는지 나란히 보여준다. Word의 트래킹 툴보다 훨씬 좋다. 

## Code is ok 

md의 장점은 코드 표현이 자유롭다는 것이다. 이미 Jupyter notebook에서 셀을 markdown으로 지정해서 코드와 코드 사이에 자유롭게 문서를 끼워 넣을 수 있다. R의 경우는 rmd라는 특화된 md 포맷이 있다. 이 정도면 md에 익숙해져서 손해볼 것은 없지 않을까? 

:feet:Jun Sok Huhh | :house:[lostineconomics.com](https://anarinsk.github.io/)









<!--stackedit_data:
eyJoaXN0b3J5IjpbOTg3NjQzMDMzXX0=
-->