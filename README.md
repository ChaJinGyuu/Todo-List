# TodoList 만들기

### 개발tool
```

react
```


## root폴더에 .prettierrc파일을 생성한다

root폴더에 .prettierrc파일을 생성한다
```javascript
{
    "arrowParens": "always",
    "semi": true,
    "singleQuote": true,
    "useTabs": false,
    "trailingComma": "all",
    "tabWidth": 2,
    "printWidth": 80
}

```

### root폴더에 jsconfig.json 파일을 생성하여 import를 위한 절대경로 설정을 한다.


```json
{
    "compilerOptions": {
        "target": "es6",
        "baseUrl": "src"
    },
    "include": ["src"]
}
```
### 기능구현하기

```
나중에 추가할 일정 항목에 대한 상태들은 모두 App 컴포넌트에서 관리한다.

App에서 useState를 사용하여 todos라는 상태를 정의하고, todos를 props로 전달한다.
```

## TodoTemplate.js 컴포넌트 만들기



react
```


## root폴더에 .prettierrc파일을 생성한다

root폴더에 .prettierrc파일을 생성한다
```javascript
{
    "arrowParens": "always",
    "semi": true,
    "singleQuote": true,
    "useTabs": false,
    "trailingComma": "all",
    "tabWidth": 2,
    "printWidth": 80
}

```

### root폴더에 jsconfig.json 파일을 생성하여 import를 위한 절대경로 설정을 한다.


```json
{
    "compilerOptions": {
        "target": "es6",
        "baseUrl": "src"
    },
    "include": ["src"]
}
```
### 기능구현하기

```
나중에 추가할 일정 항목에 대한 상태들은 모두 App 컴포넌트에서 관리한다.

App에서 useState를 사용하여 todos라는 상태를 정의하고, todos를 props로 전달한다.
```

## TodoTemplate.js 컴포넌트 만들기

```javascript
import React from 'react';
import styled from 'styled-components';

const TodoTemplate = ({ children }) => {
  return (
    <TodoWrapper>
      <AppTile>Todo List</AppTile>
      <Content>{children}</Content>
    </TodoWrapper>
  );
};
const TodoWrapper = styled.div`
  width: 512px;
  margin: 6rem auto 0;
  border-radius: 4px;
  overflow: hidden;
`;

const AppTile = styled.div`
  background: #22b8cf;
  color: #fff;
  height: 4rem;
  display: flex;
  justify-content: center;
  align-items: center;
`;

const Content = styled.div`
  background: #ffffff;
`;

export default TodoTemplate;

```

