# goバージョン
# 
# アップデートとgitのインストール
# RUN apk add --update &&  apk add git
# COPY . /go/src/sample
# WORKDIR /go/src/sample
# RUN go get -u github.com/cosmtrek/air
# RUN go get -u github.com/go-delve/delve/cmd/dlv
# CMD ["air", "-c", ".air.toml"]**

FROM golang:1.19.3-alpine
COPY . /go/src/sample
WORKDIR /go/src/sample
# アップデートとgitのインストール
RUN apk add --update &&  apk add git
RUN go get -u github.com/cosmtrek/air
RUN go get -u github.com/go-delve/delve/cmd/dlv
CMD ["air", "-c", ".air.toml"]