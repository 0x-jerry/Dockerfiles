FROM arm32v7/alpine

EXPOSE 5299

COPY BaiduPCS-Go /app/BaiduPCS-Go

VOLUME ["/root/Downloads", "/root/.config/BaiduPCS-Go"]

CMD chmod +x /app/BaiduPCS-Go && /app/BaiduPCS-Go