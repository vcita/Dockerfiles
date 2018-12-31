FROM elasticsearch:1.6.0

WORKDIR /usr/share/elasticsearch

RUN bin/plugin install elasticsearch/elasticsearch-cloud-aws/2.6.1

VOLUME /usr/share/elasticsearch/data

COPY Dockerfile /

EXPOSE 9200 9300

ENTRYPOINT ["/docker-entrypoint.sh"]

CMD ["elasticsearch"]
