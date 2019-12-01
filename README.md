# firebaseapp
Web App

 * [gxboard.web.app](https://gxboard.web.app/)
 * [gxboard.firebaseapp.com](https://gxboard.firebaseapp.com/)
 * Firebase 호스팅을 사용하여 동적 콘텐츠 제공 및 마이크로서비스 호스팅(https://firebase.google.com/docs/hosting/serverless-overview)
 * Cloud ID Free Edition 으로 50명까지 가능하여 조직(G Suite) 사용 / 도메인 인증
# 

```html
<!-- The core Firebase JS SDK is always required and must be listed first -->
<script src="/__/firebase/7.5.0/firebase-app.js"></script>

<!-- TODO: Add SDKs for Firebase products that you want to use
     https://firebase.google.com/docs/web/setup#available-libraries -->

<!-- Initialize Firebase -->
<script src="/__/firebase/init.js"></script>
```

웹 앱에 Firebase 추가
```
npm install -g firebase-tools
firebase login
firebase init
firebase use --add
firebase deploy --debug
```
 * Firebase 호스팅으로 사이트를 호스팅하려면 Firebase CLI(명령줄 도구)가 필요
 * 구글에 로그인 (이미 되어 있음)
 * 초기화

 * [Firebase 프로젝트 설정 | 서비스 계정 | Firebase Admin SDK 계정 생성](https://firebase.google.com/docs/admin/setup?hl=ko) 
 * 보안상 환경변수로 하는 것이 보안상 좋다. 
 * export GOOGLE_APPLICATION_CREDENTIALS=~/gxboard-firebase-adminsdk-.json
 
unable to verify the first certificate

 * https://www.npmjs.com/package/ssl-root-cas
 
```console
Error: Server Error. unable to verify the first certificate
export NODE_TLS_REJECT_UNAUTHORIZED=0 
```
