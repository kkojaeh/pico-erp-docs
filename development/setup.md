# 개발환경 구성

1. Git 설치
   1. https://git-scm.com/ 에서 installer 다운로드 받아 설치
2. Homebrew 설치
   1. https://brew.sh/ 에서 터미널 명령어를 복사하여 실행하여 설치
3. Redis 설치
   1. 터미널에서 ```brew install redis``` 실행하여 설치
   2. 서비스 실행설정
      1. 터미널에서 ```ln -sfv /usr/local/opt/redis/*.plist ~/Library/LaunchAgents``` 실행
      2. 터미널에서 ```launchctl load ~/Library/LaunchAgents/homebrew.mxcl.redis.plist``` 실행
   3. 동작 확인
      1. 터미널에서 ```redis-cli ping``` 실행하여 ```PONG``` 이 출력
   4. 서비스 중지 및 제거
      1. 서비스 제거 : 터미널에서 ```launchctl unload ~/Library/LaunchAgents/homebrew.mxcl.redis.plist``` 실행
      2. 레디스 제거
         1. 터미널에서 ```brew uninstall redis``` 실행
         2. 터미널에서 ```rm ~/Library/LaunchAgents/homebrew.mxcl.redis.plist``` 실행
4. Memcached 설치
   1. 터미널에서 ```brew install memcached``` 실행하여 설치
   2. 서비스 실행설정
      1. 터미널에서 ```brew services start memcached``` 실행
   3. 서비스 중지
      1. 터미널에서 ```brew services stop memcached``` 실행
   4. 서비스 제거
      1. 터미널에서 ```brew uninstall memcached``` 실행
7. IntelliJ 구성
   1. Plugins
      1. Install JetBrains plugin…
         1. Vue.js 설치
      2. Browse repositories…
         1. Spock Framework Enhancements 설치
         2. Lombok Plugin 설치
   2. Editor > Code Style
      1. Formatter control
         1. Enabled formatter markers in comments 활성화
   3. Build, Execution, Deployment > Compiler > Annotation Processors
      1. Enable annotation processing 활성화
      2. Obtain processors from project classpath 활성화
      3. Build > Rebuild Project 실행      

