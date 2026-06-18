ARG BUILD_FROM
FROM $BUILD_FROM

RUN apk add --no-cache python3 py3-pip \
 && pip3 install --no-cache-dir paho-mqtt --break-system-packages

COPY km140f.py /km140f.py
COPY run.sh    /run.sh
RUN chmod +x /run.sh

CMD ["/run.sh"]
