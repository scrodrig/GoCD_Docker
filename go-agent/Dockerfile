FROM gocd/gocd-agent-centos-7:v17.12.0
LABEL Description="go-agent" Version="1.0"
RUN yum update -y
RUN curl --location https://rpm.nodesource.com/setup_7.x | bash -
RUN yum install -y nodejs
RUN yum install -y gcc-c++ make
RUN curl -fsSL https://get.docker.com/ | sh
ENV GO_SERVER_IP_ADDRESS 10.71.23.144
ENV GO_SERVER_AGENT_PORT 3010
ENV GO_SERVER_URL https://${GO_SERVER_IP_ADDRESS}:${GO_SERVER_AGENT_PORT}/go
