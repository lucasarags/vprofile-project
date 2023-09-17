FROM httpd:2.4

LABEL "Project"="Vprofile"
LABEL "Author"="Arags"

RUN rm -rf /usr/local/apache2/htdocs/*
COPY apachevproapp.conf /usr/local/apache2/conf/extra/vproapp.conf

EXPOSE 80