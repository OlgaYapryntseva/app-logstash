FROM docker.elastic.co/logstash/logstash:8.3.3

COPY ./logstash/config/logstash.yml /usr/share/logstash/config/logstash.yml
COPY ./logstash/pipeline /usr/share/logstash/pipeline

ENV LS_JAVA_OPTS="-Xmx256m -Xms256m"
ENV PORT=5000

CMD ["logstash", "-f", "/usr/share/logstash/pipeline/logstash.conf"]
