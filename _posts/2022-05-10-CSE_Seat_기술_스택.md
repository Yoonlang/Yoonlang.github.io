---
layout: post
title: CSE Seat 기술 스택에 대해
---

CSE Seat의 프론트엔드 개발자로 개발하며 사용한 기술과 배제한 기술에 대해 이야기하고자 한다.

### 토픽
* Next.js
* Recoil
* Typescript


#### Next.js
Next.js를 선택함에 있어 선택지가 3가지 있었다.
1. Next.js
2. React
3. HTML, CSS, vanilla JS

이 중 Next.js를 선택한 이유는
1. 컴포넌트 기반의 React를 사용하며 SSR로 구현해 보고 싶었고
2. 이를 구현하는 데 있어서 한정된 시간 상 편리하고 유저 풀이 커야 개발이 원활하기 때문이다.

기존에 다른 가벼운 프로젝트에서 React로 CSR을 구현해 보았고, 사람들이 Next.js가 좋다는 이유를 직접 경험해서 알고 싶었다.


#### Recoil
Recoil을 선택함에 있어 선택지가 3가지 있었다.
1. Redux
2. Recoil
3. context API

이 중 context API는 우선 배제했다. context API는 상태 관리를 목적으로 만들어진 것이 아니기 때문이다.
Redux와 Recoil 중 Recoil을 선택한 이유는 두 가지이다.
1. Recoil은 Meta에서 직접 지원하는 라이브러리이다. 따라서 안정화가 되고 시간이 지나면 Recoil의 빈도가 더욱 커질 것이다.
2. Recoil의 진입장벽이 Redux보다 낮다.
    이번 프로젝트에서 상태 관리 라이브러리를 처음 경험하는 나에겐 진입장벽이 상대적으로 낮은 Recoil이 더욱 매력적이었다.

#### Typescript
Typescript는 처음 계획상 채택했지만 개발 도중 포기했다.
Typescript를 채택한 이유
1. 정적으로 Type을 검사할 수 있는 것이 매력적이라 느꼈다.
2. 현대의 프론트엔드 개발자로서 Typescript가 필수라고 느꼈기에 이번 프로젝트에서 경험해 보고 싶었다.

개발 도중 Typescript를 배제한 이유
1. 프로젝트 종료 기간이 정해져있는데, Typescript 때문에 시간이 지체됐다.
    3월 말까지는 서비스 개발이 완료되어야 했는데, Typescript뿐만 아니라 Next.js, Recoil 또한 처음 경험해 보는 것이라 어설픈 실력으로 Typescript를 쓰기에 굉장히 난해했다. 
2. Typescript가 필수는 아니다.
    프로젝트 규모가 크지 않아서 Type에 대한 고려를 충분히 한다면 오류를 최소화할 수 있을 것이라 판단했다. 따라서 Typescript를 배제했다.


### 마무리
이번 프로젝트를 통해 다양한 것을 시도하며 좋은 경험이 되었다고 느낀다. 다음 프로젝트를 한다면 Next.js 대신 React 18의 SSR 기능을 사용해 프레임워크를 덜고 싶다. 또한 Typescript를 제대로 공부해서 적용해 보고 싶다. 조금 더 욕심을 내자면 Jest를 통한 테스팅도 해보고 싶다.