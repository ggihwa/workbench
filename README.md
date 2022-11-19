## 1. eslint

#### 코드의 항상성을 유지와 버그를 피하기 위해 자바스크립트 코드에서 패턴을 정의하고 리포팅하는 툴.

---

### Install

npm init @eslint/config  
여러가지를 대답하면 .eslintrc 파일이 생성된다.  
질문내에서 필요한 패키지들을 설치할 수 있다.

### Configuration

```
env
extends - 미리 설정한 규칙모음.
overrides - 특정 파일들에서 규칙을 오버라이드할 수 있게 설정할 수 있다.
parserOptions
plugins - eslint에서 정의한 규칙 이외에 새롭게 규칙을 추가할 수 있다.
rules - 규칙들 설정
```

[\*eslint rules link](https://eslint.org/docs/latest/rules/)

### airbnb

## 2. prettier

---

### Install

npm install -D prettier eslint-config-prettier eslint-plugin-prettier

.eslintrc에 plugin, config 설정  
eslint-config-prettier : eslint 규칙 중에 prettier와 상충되는 옵션을 모두 비활성화 한다.  
eslint-plugin-prettier : prettier 규칙을 eslint에 리포팅하도록 한다.

*인텔리제이는 prettier 플러그인을 설치하면 on save option에 따라 code formatter 로 기본 동작으로 작동함.

## 3. fix

---

eslint src/* --fix

* autofix가 제공되는 규칙들만 수정된다. ([*eslint rules link](https://eslint.org/docs/latest/rules/) 참고)
* prettier 설정도 함께 수정된다.

npx prettier --write . (npx prettier --check .)

## 4.husky & lint-staged

---

### install

npx mrm@2 lint-staged (참고: https://prettier.io/docs/en/precommit.html)   
*작동이 잘 안되면 기본은 js로 되어 있으므로 lint-staged에 설정되어 있는 확장자 체크해보자. 