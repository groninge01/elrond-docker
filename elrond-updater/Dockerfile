FROM ubuntu:18.04

ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update -y && apt-get upgrade -y && apt install -y  apt-utils wget git docker.io curl
ADD libwasmer_runtime_c_api.so /lib/libwasmer_runtime_c_api.so
ADD updater.sh /opt/updater.sh
RUN chmod +x /opt/updater.sh
CMD ["/opt/updater.sh"]
