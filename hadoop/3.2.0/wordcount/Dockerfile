FROM adityap174/poc:hadoop-base-2.0.4-hadoop-3.2.0-java8

MAINTAINER Ivan Ermilov <ivan.s.ermilov@gmail.com>

COPY WordCount.jar /opt/hadoop/applications/WordCount.jar

ENV JAR_FILEPATH="/opt/hadoop/applications/WordCount.jar"
ENV CLASS_TO_RUN="WordCount"
ENV PARAMS="/input /output"

ADD run.sh /run.sh
RUN chmod a+x /run.sh

CMD ["/run.sh"]
