FROM jboss/wildfly:19.0.0.Final

ADD https://downloads.mariadb.com/Connectors/java/connector-java-1.5.9/mariadb-java-client-1.5.9.jar /opt/jboss/wildfly/modules/system/layers/base/org/mariadb/jdbc/main/
COPY librerias/module.xml /opt/jboss/wildfly/modules/system/layers/base/org/mariadb/jdbc/main/
ADD aplicacion/Aplicacion.war /opt/jboss/wildfly/standalone/deployments/

RUN /opt/jboss/wildfly/bin/add-user.sh admin Admin#123 --silent
