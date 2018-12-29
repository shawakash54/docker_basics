# FROM ubuntu:16.04
# RUN apt-get update
# RUN apt-get -y install curl
# RUN curl https://google.com | wc -c > google_count
# ENTRYPOINT echo google is this big; cat google_count


FROM ubuntu:16.04 as builder
RUN apt-get update
RUN apt-get -y install curl
RUN curl https://google.com | wc -c > google_count


FROM alpine
COPY --from=builder /google_count /google_count
ENTRYPOINT echo google is this big; cat google_count


