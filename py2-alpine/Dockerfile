FROM python:2-alpine
MAINTAINER  <https://github.com/naumvd95>

ENV PYLINT_VERSION=1.7.2

RUN apk add --no-cache --virtual .run-deps \
    && pip install flake8 flake8-docstrings pylint

COPY setup.sh /

ENTRYPOINT ["/setup.sh"]
CMD ["pylint"]
