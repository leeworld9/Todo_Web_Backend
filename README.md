# Todo_Web_Application

## 1. 구현 목표 및 목적
- **다수의 사용자를 지원하는** 웹 기반의 Todo 애플리케이션을 구현하고 배포
  - 기능보다는 프론트엔드/백엔드 개발 전반에 대한 경험을 메인으로 함.
- **확장 가능한 서비스 개발 및 운영에 대해 전반적으로 경험**
- **프론트엔드와 백엔드 서버가 분리된 아키텍처 경험 및 구현**

## 2. 구체적인 사용 기술
- 프론트엔드 : React.js 16.14.0 (Node.js 14)
- 백엔드 : Spring Boot 2.5.10
- 인증 : JWT(백엔드), 로그인 상태유지(프론트엔드)
- 배포 : AWS
    - Elastic Beanstalk 사용
      - 로드 밸런서, 오토 스케일링 그룹 등 스케일링에 필요한 서비스 자동 구성
      - RDS(mysql) 환경 추가
      - 개발(local, h2), 프로덕션(ec2, mysql) 환경을 나눔
    - ~~Router 53을 통한 도메인 구매~~ (생략)
    - ~~HTTPS 인증서 발급~~ (생략)

## 3. Todo 웹 애플리케이션 아키텍처
![Alt text](https://i.ibb.co/1mQB31f/2022-05-04-2-04-26.png)

## 4. 추후 해보고 싶은 내용
 - 자동으로 환경이 구성되는 Elastic Beanstalk 말고 다른 방법으로 환경 구성.
 - CI/CD 환경 구성 및 적용.
 - Swagger를 사용한 API 문서 자동화.
 - TDD(테스트 주도 개발) 적용.

## 5. 참고
 - http://www.yes24.com/Product/Goods/103768882
 - https://thecodinglog.github.io/java/2020/12/15/java-generic-wildcard.html
 - http://yoonbumtae.com/?p=2773
 - https://devfunny.tistory.com/364
 - https://brunch.co.kr/@heracul/3
 - https://d-life93.tistory.com/309
 - https://velog.io/@kcdoggo/Switch-is-not-exported-from-react-router-dom-%EC%97%90%EB%9F%AC
