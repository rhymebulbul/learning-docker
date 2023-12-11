# Yo this is my second docker image

FROM ubuntu

COPY . /app

ENV curl_bin="curl=7.85.0"

#ARG curl_bin="curl"

RUN apt -y update && apt -y install "$curl_bin"

CMD ["--argument_optional"]

ENTRYPOINT ["/app/app.sh", "--argument_fixed"]

