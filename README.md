# 에러 재현법

프로젝트의 루트에서
`bundle install` 을 해주세요.

`cd ios`
`bundle exec pod install`

을 하게 되면 `Processing RNNotiflyReactNativeSdkSpec`으로 시작되는 notifly-sdk 에서 에러가 남을 확인 할 수 있었습니다.

관련해서 임시적인 해결법은
`node_modules/notifly-sdk/package.json` 파일에서 codegenConfig 를 지우면 해결이 됩니다.