FROM arm32v7/alpine

EXPOSE 5299

WORKDIR /app

COPY BaiduPCS-Go /app

VOLUME ["/root/Downloads", "/root/.config/BaiduPCS-Go"]

CMD chmod +x ./BaiduPCS-Go && ./BaiduPCS-Go