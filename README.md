## SonarQube-Install
#### Kubernetes를 이용한 SonarQube 설치

---

## 파일 설명

### postqres Directory

- postqres-configmap.yaml : Postqres 설정 값 - username, database, password
- postqres-deploy.yaml : Postqres 배포를 위한 Deployment
- postqres-pvc.yaml : Postqres 데이터 저장을 위한 Volume 요청 Pvc
- postqres-svc.yaml : Postqres가 SonarQube와 통신하기 위한 ClusterIP Service

---

### sonarqube Directory

- ingress-sonardashboard.yaml : SonarQube DashBoard 외부 노출을 위한 Ingress
- sonar-configmap.yaml : SonarQube를 Postqres와 연동하기 위한 설정 값 - Postqres Url, Postqres username, Postqres password
- sonar-deploy.yaml : SonarQube 배포를 위한 Deployment
- sonar-pvc.yaml : SonarQube 데이터, Plugin 저장을 위한 Volume 요청 Pvc
- sonar-svc.yaml : SonarQube-Ingress, SonarQube-Postqres 통신을 위한 ClusterIP Service
