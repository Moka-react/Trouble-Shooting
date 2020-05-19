# React Study Documentation and Question

리액트 스터디에서 **질문을 하는 방법**에 대해 다음 양식을 지켜주세요.

1.  `GitHub에 Issue를 등록`해주세요. 매번 같은 질문을 대답해주기에 한계가 있어 질문과 답변을 공유하는 목적입니다.

2.  질문을 올리기 전에 먼저 `GitHub Issue를 확인`해주세요. 그 질문에 대한 그 동안의 답변을 빠르게 얻으실 수 있을 것 입니다.

3.  답변을 안해주더라도 본인이 먼저 답을 찾았을 경우에 해당 Issue에 답에 대한 공부 내용을 기록해주면 좋을 것 같아요. 다음에 같은 고민을 하는 사람에게 큰 도움이 될 것 입니다.

## Issue를 남기는 방법

`GitHub Repository > Issue > New Issue`를 통해 Issue를 생성할 수 있습니다. 최대한 다음과 같은 양식은 반드시 지켜주세요. 서로 같이 질문하고 배워가면서 상대방을 배려하는 질문법을 배워나갑시다.

### Issue title
이슈 리스트에서도 확인 할 수 있도록 어떤 문제인지 한줄로 명확히 나타내주세요!

아래부터는 이슈의 예시입니다.

---

### 부가 설명
내 코드에서 문법적인 문제를 모르겠습니다. 알려주세요


### 에러 문구
```
Syntax error: Unexpected token (48:18)

   46 |   LOAD_BLOCK_USERS_SUCCESS,
   47 |   LOAD_BLOCK_USERS_FAILURE,
> 48 | )<undefined, DataProps, AxiosError>();
                         ^
```
### 코드 구현 부
```
www.github.com/[my_github]
```
또는
```typescript
import axios, { AxiosError } from 'axios';

interface IData {
  total: number;
  items: Array<number>;
}
export const loadBlockUserRequestAsync = createAsyncAction(
  LOAD_BLOCK_USERS,
  LOAD_BLOCK_USERS_SUCCESS,
  LOAD_BLOCK_USERS_FAILURE,
)<undefined, DataProps, AxiosError>();
```
---

### Project Dependencies

- typescript Version: "^3.8.2"
- typesafe-actions Version: "^5.1.0"
- tsconfig.json:

  ```json
  {
    "compilerOptions": {
      "esModuleInterop": true,
      "strict": true,
      "types": ["react"],
      "baseUrl": ".",
      "lib": [
        "DOM",
        "ES5",
        "ES2015",
        "ES2016",
        "ES2017",
        "ES2018",
        "ES2019",
        "ES2020"
      ],
      "jsx": "react"
    },
    "exclude": ["node_modules"]
  }
  ```

---

### Environment (optional)

- OS:MAC osx catalina
- Node Version: 10.15.3
