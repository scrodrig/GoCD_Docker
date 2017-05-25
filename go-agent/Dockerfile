FROM gocd/gocd-agent-centos-7:v17.4.0
LABEL Description="go-agent" Version="1.0"
RUN yum update
RUN curl --location https://rpm.nodesource.com/setup_7.x | bash -
RUN yum install -y nodejs
RUN yum install -y gcc-c++ make
ENV GO_SERVER_IP_ADDRESS 10.71.23.152
ENV GO_SERVER_AGENT_PORT 3010
ENV GO_SERVER_URL https://${GO_SERVER_IP_ADDRESS}:${GO_SERVER_AGENT_PORT}/go
