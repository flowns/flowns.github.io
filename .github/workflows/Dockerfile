FROM python:3.12-rc-alpine

ENV AWSCLI_VERSION='1.29.18'

RUN pip install --upgrade pip
RUN pip install pyyaml~=6.0
RUN pip install --quiet --no-cache-dir awscli==${AWSCLI_VERSION}

COPY ./entrypoint.sh /entrypoint.sh
RUN chmod +x entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
