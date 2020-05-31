FROM arm32v7/golang:alpine AS build
RUN apk add git
WORKDIR /go/src/swirl/
ADD . .
ENV GO111MODULE on
RUN CGO_ENABLED=0 go build -ldflags "-s -w"

FROM arm32v7/alpine
LABEL maintainer="cuigh <noname@live.com>"
WORKDIR /app
RUN apk add --no-cache ca-certificates
COPY --from=build /go/src/swirl/swirl .
COPY --from=build /go/src/swirl/config ./config/
COPY --from=build /go/src/swirl/assets ./assets/
COPY --from=build /go/src/swirl/views ./views/
EXPOSE 8001
ENTRYPOINT ["/app/swirl"]
