# BE_toy_project

백엔드 토이 프로젝트
Koa 사용 

### 1.도식화

main.js

<br> ![main](https://user-images.githubusercontent.com/59908043/137437457-b9fb8822-2350-4934-aeae-e297844f3b34.PNG)

Schema(PostSchema와 UserSchema)

<br> ![Schema](https://user-images.githubusercontent.com/59908043/137437752-4e8f80f3-cc92-470d-8fa3-bb4b2c0132e1.PNG)

auth

<br> ![auth](https://user-images.githubusercontent.com/59908043/137437908-b7cf4af3-f0f7-453e-ac81-e6aa92aefdb4.PNG)

posts

<br> ![posts](https://user-images.githubusercontent.com/59908043/137437923-cbeb357b-1520-4489-b1cf-acc5b1c6bff9.PNG) 

### 2. 배운점 메모
<br>start:dev: nodemon을 통해 src 디렉터리를 보다가 파일이 변경되면 재시작
<br>REST API: 클라이언트가 DB에 직접 접속하여 데이터를 변경하면 안되므로 REST API를 사용,get post delete put patch 
<br>컨트롤러: 라우트 처리 함수들을 모아 놓은 파일
<br>koa-bodyparser: request body에 JSON형식으로 데이터를 넣어주면, 이를 파싱하여 서버에서 사용할 수 있게 함
<br>module.exports: 다른 파일에서 사용할 수 있게 한다(exports 대체 가능)
<br>ctx: Context의 줄임말로 웹 요청과 응답에 관한 정보를 지니고 있다
<br>save()를 실행해야 데이터베이스에 저장(async/await 사용)
<br>find()함수 호출한 후 exec()를 붙여야 서버에 쿼리 요청
<br>@hapi/joi: 내용이 자기가 만든 스키마의 형식에 맞는지 확인할때 사용
<br>bodyParser가 deprecate되어서 koa-bodyparser사용
<br>인스턴스 메서드를 작성할 때, this(인스턴스)를 사용하게 된다면 화살표 함수가 아닌 function을 사용하여 구현해야한다. 스태틱 함수에서 this는 모델을 가리킴
<br>jwt를 이용하여 토큰 생성
<br>MongoDB에서 조회한 ID값은 문자열과 비교할 때는 .toString()을 써야한다.
<br>ctx.state: 미들웨어 및 프론트 엔드로 정보를 전달하기 위한 권장 네임 스페이스