FROM amazon/opendistro-for-elasticsearch:0.7.1

# Override config, otherwise plug-in install will fail
COPY ./config /usr/share/elasticsearch/config

WORKDIR /usr/share/elasticsearch

# Set environment
ENV DISCOVERY_SERVICE elasticsearch-discovery

# Kubernetes requires swap is turned off, so memory lock is redundant
ENV MEMORY_LOCK false

