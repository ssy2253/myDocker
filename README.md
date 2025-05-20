```markdown
# Ubuntu Docker Image

이 Dockerfile은 `ubuntu:22.04` 이미지를 기반으로 `/xxxxx` 디렉토리를 생성합니다.

## 📁 디렉토리 구조

```

Dockerfile
README.md

````

## ⚙️ Dockerfile 내용

```dockerfile
FROM ubuntu:22.04
RUN mkdir /xxxxx
````

## 🚀 빌드 방법

```bash
docker build -t my-ubuntu-image .
```

## ▶️ 실행 방법

```bash
docker run -it --name my-ubuntu-container my-ubuntu-image
```

## 📂 설명

* `FROM ubuntu:22.04` : 우분투 22.04 이미지를 기반으로 함
* `RUN mkdir /xxxxx` : `/xxxxx` 디렉토리를 생성함

---

## 📝 참고

이 이미지는 테스트 및 교육용으로 사용하기 위한 단순한 예제입니다.

```

---

필요하다면 `RUN apt update`, `COPY`, `CMD`, `WORKDIR` 같은 더 많은 명령어가 포함된 예시로 확장해드릴 수도 있습니다.  
추가 기능이 필요한 경우 말씀해주세요!
```
