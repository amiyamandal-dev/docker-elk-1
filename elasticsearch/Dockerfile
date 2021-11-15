ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/elasticsearch/elasticsearch:${ELK_VERSION}
RUN mkdir -p /usr/share/elasticsearch/data
RUN chmod 777 -R /usr/share/elasticsearch/
RUN chown -R elasticsearch:elasticsearch /usr/share/elasticsearch/
# USER root
RUN elasticsearch-plugin install analysis-icu

# Add your elasticsearch plugins setup here
# Example: RUN elasticsearch-plugin install analysis-icu
