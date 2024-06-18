# Используем официальный образ Logstash
FROM docker.elastic.co/logstash/logstash:8.3.3

# Копируем конфигурационные файлы Logstash
COPY logstash/config/logstash.yml /usr/share/logstash/config/logstash.yml
COPY logstash/pipeline /usr/share/logstash/pipeline

# Запуск Logstash при старте контейнера
CMD ["logstash", "-f", "/usr/share/logstash/pipeline"]



