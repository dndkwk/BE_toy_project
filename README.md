# BE_toy_project

백엔드 토이 프로젝트
Koa 사용 

<br>start:dev: nodemon을 통해 src 디렉터리를 보다가 파일이 변경되면 재시작
<br>REST API: 클라이언트가 DB에 직접 접속하여 데이터를 변경하면 안되므로 REST API를 사용,get post delete put patch 
<br>컨트롤러: 라우트 처리 함수들을 모아 놓은 파일
<br>koa-bodyparser: request body에 JSON형식으로 데이터를 넣어주면, 이를 파싱하여 서버에서 사용할 수 있게 함
<br>ctx.status와 ctx.body의 의미 알아보기
<br>module.exports의 의미