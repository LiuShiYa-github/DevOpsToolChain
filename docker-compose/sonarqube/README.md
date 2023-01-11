## 参考
[官方文档](https://docs.sonarqube.org/latest/)

## 默认账密
```shell
login: admin
password: admin
```
## 启动扫描
```shell
docker run \
    --rm \
    -e SONAR_HOST_URL="http://10.0.0.30:9000" \
    -e SONAR_SCANNER_OPTS="-Dsonar.projectKey=flaskblog" \
    -e SONAR_LOGIN="aca6cbe0ad0994983ac48a42285ad21cf07dea90" \
    -v "$PWD:/usr/src" \
    sonarsource/sonar-scanner-cli
```
