# ENTITY 생성기 사용방법

typeorm 에서 사용할 entity 를 데이터베이스에서 접속하여 생성합니다.<br>
자세한 설명은 아래 npm 사이트를 참조 합니다.<br>

[typeorm-model-generator](https://www.npmjs.com/package/typeorm-model-generator) Generates models for TypeORM from existing databases. Supported db engines:

* Microsoft SQL Server
* PostgreSQL
* MySQL
* MariaDB
* Oracle
* SQLite


## 모듈 설치

```bash
# install generator
$ npm install -g typeorm-model-generator
```

## 생성기 실행

사용하는 데이터베이스에 맞게 설정하여 실행합니다.

> engine type 선택:<br>"mssql", "postgres", "mysql", "mariadb", "oracle", "sqlite"

```bash
# Running generator
$ typeorm-model-generator -h {HOST} -d {DATABASE} -p {PORT} -u {USER} -x {PASSWORD} -e {ENGINE TYPE} -o {OUTPUT FOLER}
```


## 프로젝트 폴더 이동
생성된 파일명을 프로젝트 폴더에 이동 시 확장자를 변경합니다. (~~~.entity.ts)
```bash
# ex> Users.ts
# 프로젝트 엔티티 폴더 이동 > src/entities/Users.entity.ts
```