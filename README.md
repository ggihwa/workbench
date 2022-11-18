## eslint
#### 코드의 항상성을 유지와 버그를 피하기 위해 자바스크립트 코드에서 패턴을 정의하고 리포팅하는 툴.
<hr />
npm init @eslint/config   
여러가지를 대답하면 .eslint.rc 파일이 생성된다.    
질문내에서 필요한 패키지들을 설치할 수 있다.   

````
env
extends - 미리 설정한 규칙모음. 
overrides - 특정 파일들에서 규칙을 오버라이드할 수 있게 설정할 수 있다.
parserOptions
plugins - eslint에서 정의한 규칙 이외에 새롭게 규칙을 추가할 수 있다.
rules - 규칙들 설정
````

### airbnb




      
## prettier
<hr />
eslint-config-prettier : eslint 규칙 중에 prettier와 상충되는 옵션을 모두 비활성화 한다.     
eslint-plugin-prettier : prettier 규칙을 eslint에 리포팅하도록 한다.
