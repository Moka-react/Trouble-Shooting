---
name: Trouble-Shooting template
about: Please follow the issue form as much as possible.
title: ''
labels: ''
assignees: ''

---

### 부가 설명
> 이곳에 설명을 작성해주세요
내 코드에서 문법적인 문제를 모르겠습니다. 알려주세요.


### 에러 문구
> 에러 문구를 작성해주세요
```
Syntax error: Unexpected token (48:18)

   46 |   LOAD_BLOCK_USERS_SUCCESS,
   47 |   LOAD_BLOCK_USERS_FAILURE,
> 48 | )<undefined, DataProps, AxiosError>();
                         ^
```
### 코드 구현 부
> 에러난 부분의 코드 또는 전체코드 적어주세요 
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
> 프로젝트 설정값을 적어주세요
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
> 프로젝트가 어떤 환경에서 실행 됐는지 적어주세요
- OS:MAC osx catalina
- Node Version: 10.15.3
