# Image-Hoster

Spring Boot image hosting app (register, login, upload/edit/delete images with tags).

## Prerequisites

- JDK 17 (`brew install openjdk@17`)
- PostgreSQL running locally with database `imageHoster`

```bash
createdb imageHoster
```

DB connection defaults (in `JpaConfig` / `persistence.xml`):

- URL: `jdbc:postgresql://localhost:5432/imageHoster`
- User: your macOS username (`shashesi2712`)
- Password: empty (local trust auth)

## Run

```bash
export JAVA_HOME=/opt/homebrew/opt/openjdk@17/libexec/openjdk.jdk/Contents/Home
export PATH="$JAVA_HOME/bin:$PATH"
mvn spring-boot:run
```

Open [http://localhost:8080](http://localhost:8080).

Do **not** run `ImageHosterApplication` via the plain Java “Run” button without Maven — Spring dependencies will be missing.
