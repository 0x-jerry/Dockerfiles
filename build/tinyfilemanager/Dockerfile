FROM arm32v7/php

WORKDIR /app

EXPOSE $PORT

COPY src /app

VOLUME [ "/app/folder" ]

CMD php -S 0.0.0.0:$PORT tinyfilemanager.php