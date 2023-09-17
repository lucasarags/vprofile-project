# build the artifact
FROM openjdk:11 AS BUILD_IMAGE
RUN apt update && apt install maven -y
RUN git clone https://github.com/lucasarags/vprofile-project.git \
    && cd vprofile-project \
    && git checkout docker \
    && mvn install

# be having the artifact
FROM tomcat:9-jre11
LABEL "Project"="Vprofile"
LABEL "Author"="Arags"
RUN rm -rf /usr/local/tomcat/webapps/*
COPY --from=BUILD_IMAGE vprofile-project/target/vprofile-v2.war /usr/local/tomcat/webapps/ROOT.war

EXPOSE 8080
CMD ["catalina.sh","run"]