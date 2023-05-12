## SonarQube-Install
#### Kubernetes를 이용한 SonarQube 설치

---

## 파일 설명

### postqres Directory

- postqres-configmap.yaml : Postqres 설정 값 - username, database, password
- postqres-deploy.yaml : Postqres 배포
- postqres-pvc.yaml : Postqres 데이터 저장을 위한 Volume 
- postqres-svc.yaml : Postqres가 Sonarqube와 통신하기 위한 ClusterIP Service

---

### sonarqube Directory

- ingress-sonardashboard.yaml : SonarQube DashBoard 외부 노출을 위한 Ingress
