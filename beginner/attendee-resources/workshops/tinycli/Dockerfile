FROM ubuntu:16.04

LABEL maintainer="craigdcn@gmail.com"
LABEL version="0.0.1"
LABEL description="k8s workshop"

RUN apt-get update && apt-get install -y curl

ADD message.txt /message.txt
ADD run.sh /run.sh

RUN chmod a+x /run.sh

ENTRYPOINT ["/run.sh "]

CMD ["https://httpbin.org/user-agent"]

