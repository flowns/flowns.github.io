FROM python:3.9-alpine

ENV AWSCLI_VERSION='1.24.3'

RUN pip install --quiet --no-cache-dir awscli==${AWSCLI_VERSION}

COPY ./entrypoint.sh /entrypoint.sh
RUN chmod +x entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
