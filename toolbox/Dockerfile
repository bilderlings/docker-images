FROM google/cloud-sdk:alpine

RUN apk add --no-cache curl openssh \
    zip gzip tar jq rsync which bash coreutils

RUN addgroup -g 1000 -S toolbox && \
    adduser -u 1000 -S toolbox -G toolbox

USER 1000:1000

