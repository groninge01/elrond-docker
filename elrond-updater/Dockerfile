FROM elrond:botn
ADD libwasmer_runtime_c_api.so /lib/libwasmer_runtime_c_api.so
ADD updater.sh /opt/updater.sh
ADD  --chown=elrond:elrond updater.sh /opt/updater.sh
RUN chmod +x /opt/updater.sh
CMD ["/opt/updater.sh"]
