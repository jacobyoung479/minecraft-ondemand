# version 1.2.0
# docker pull jacobyoung479/minecraft-ecsfargate-watchdog

FROM amazon/aws-cli

RUN yum install -y net-tools jq nmap-ncat && \
    yum clean all

COPY ./watchdog.sh .

ENTRYPOINT ["./watchdog.sh"]
