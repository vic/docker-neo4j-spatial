FROM thetallgrassnet/alpine-neo4j:3.0.0-M04
MAINTAINER Victor Borja vborja@apache.org

ENV SPATIAL_RELEASE 0.23-neo4j-3.0.4
ENV SPATIAL_RELEASES_URL https://github.com/neo4j-contrib/m2/blob/master/releases/org/neo4j/neo4j-spatial
ENV SPATIAL_PLUGIN_JAR neo4j-spatial-${SPATIAL_RELEASE}-server-plugin.jar
ENV SPATIAL_PLUGIN_URL ${SPATIAL_RELEASES_URL}/${SPATIAL_RELEASE}/${SPATIAL_PLUGIN_JAR}

RUN wget -O /var/lib/neo4j/plugins/${SPATIAL_PLUGIN_JAR} ${SPATIAL_PLUGIN_URL}?raw=true
