FROM devopsfaith/krakend:latest

ARG AUDIENCE
ARG JWK_URL
ARG COMPONENT_HOST


COPY krakend.template.json /etc/krakend/krakend.template.json

RUN apk add gettext && export AUDIENCE && export JWK_URL && export COMPONENT_HOST && envsubst < /etc/krakend/krakend.template.json > /etc/krakend/krakend.json
