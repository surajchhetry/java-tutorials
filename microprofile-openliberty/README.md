# Build
mvn clean package && docker build -t com.github.surajchhetry.javatutorials/microprofile-openliberty .

# RUN

docker rm -f microprofile-openliberty || true && docker run -d -p 8080:8080 -p 4848:4848 --name microprofile-openliberty com.github.surajchhetry.javatutorials/microprofile-openliberty 