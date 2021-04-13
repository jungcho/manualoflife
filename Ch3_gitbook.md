---
description: GitBook을 이용한 책쓰기 사례를 소개한다.
---

# GitBook을 이용한 책쓰기

## 절차

GitHub와 GitBook은 어떻게 연계를 하는가?

모르겠으면 아래의 링크를 찾아간다. [https://www.youtube.com/watch?v=e9DMxI\_XOPI](https://www.youtube.com/watch?v=e9DMxI_XOPI)

GibBook 왼쪽 메뉴 Intergrations에서 GitHub를 클릭한다.

책을 쓸 때는 질문을 한다.

GitHub와 연결을 해봤다. 테스트해보

## GitBook과 GitHub 연결하기

깃북과 갓헙을 연결해야 될 것 같다. 왜냐하면, 그래야지 오프라인 노트북에서 글을 쓰고, 이 글을 온라인에 통합시킬 수 있을 것이다. 반대로 온라인에서 쓰고 오프라인에서 편집하는 것도 하나의 좋은 방법이 될 것 같다.

다음의 [링크](https://docs.gitbook.com/integrations/github)에 설명이 잘되어있다. 깃북에서 편집을 한다면, Integrations에서 GitHub의 Edit configuration에서 리포지토리로 링크를 건다. 이후에는 깃헙에 가서 Pull을 요청한다. 내가 이것을 몰랐던 것 같다.

깃헙에서 편집하고 나서는 어떻게 해야 하는가? 지금 깃헙에서 편집하고 있는데 테스트를 해보자 . 데스크톱에서 Commit을 하고, Push를 한다. GitHub repository까지는 잘 들어간다. 이후에는... 해야할 것 같다.

## 브랜치 문제해결

내가 어렵게 푼 문제 중 하나는 브랜치가 서로 꼬여 있었던 것이다. Github는 기본적으로 `main`브랜치인 반면, GitBook은 `master` 브랜치에 저장이 된다. 이것때문에 GitBook 웹에서의 편집과, GitHub Desktop에서의 편집이 각자 진행이 되었던 것이다.

해결은 두 브랜치를 병합함으로 해결이 되었다.







