# 🛠️ Spring Boot JPA + H2 Demo 프로젝트 요약

## 📦 프로젝트 정보
- **Framework**: Spring Boot 3.5.0
- **Build Tool**: Gradle
- **Java Version**: 17
- **Database**: H2 (in-memory)
- **ORM**: Spring Data JPA
- **Lombok**: 코드 축약용

---


## 📘 H2 Console

- 접속: 
  - 로컬 : http://localhost:로컬포트번호/h2-console
  - 배포 후 : http://<ec2-IP>:8080/h2-console

- JDBC URL: jdbc:h2:mem:testdb

- username: sa

- password: (빈칸)

---

## ✅ 전체 워크플로우 요약

1. GitHub Actions runner : Java 17 설치

2. GitHub Actions runner: application.properties 생성

3. GitHub Actions runner: 프로젝트 빌드 (./gradlew build)

4. GitHub Actions runner: Docker 이미지 빌드 및 ECR에 Push

5. EC2 서버에 SSH 접속

6. 기존 프로세스 및 컨테이너 정리

7. 최신 Docker 이미지 Pull 및 컨테이너 실행



