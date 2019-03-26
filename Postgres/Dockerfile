FROM postgres:10-alpine
#RUN mkdir /docker-entrypoint-initdb.d/
#COPY initdb.sql /docker-entrypoint-initdb.d/
COPY my-postgres.conf /usr/local/share/postgresql/postgresql.conf
#ENV POSTGRES_USER statEntityUser
#ENV POSTGRES_PASSWORD test123
#ENV POSTGRES_DB StatisticalRestService


ENTRYPOINT ["docker-entrypoint.sh"]
EXPOSE 5432
CMD [ "postgres" ]