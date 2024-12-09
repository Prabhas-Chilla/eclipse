from openjdk:17-jdk-slim
workdir /usr/src/external
copy ./src /usr/src/external/src
copy .classpath /usr/src/external
run mkdir bin && javac -d bin/src/external/*.java src/module-info.java
cmd ["java","external.Main"]
