# Image-Hoster

Spring Boot image hosting app (register, login, upload/edit/delete images with tags).

## Prerequisites

- JDK 17 (`brew install openjdk@17`)
- PostgreSQL running locally with database `imageHoster`

```bash
createdb imageHoster
```

DB settings via env vars (optional):

- `DB_URL` — default `jdbc:postgresql://localhost:5432/imageHoster`
- `DB_USER` — default `shashesi2712`
- `DB_PASSWORD` — default empty

## Run

```bash
export JAVA_HOME=/opt/homebrew/opt/openjdk@17/libexec/openjdk.jdk/Contents/Home
export PATH="$JAVA_HOME/bin:$PATH"
# export DB_PASSWORD='your-password'   # if needed
mvn spring-boot:run
```

Or build and run the JAR:

```bash
mvn -DskipTests package
java -jar target/ImageHoster-1.0-SNAPSHOT.jar
```

Open [http://localhost:8080](http://localhost:8080).
