# PDF.js Viewer

[PDF.js](https://github.com/mozilla/pdf.js) [Viewer](https://mozilla.github.io/pdf.js/web/viewer.html) dockerized. 

## Deploy

```bash
docker buildx build --platform linux/arm,linux/arm64,linux/amd64 -f Dockerfile -t douguohai/pdfjs-viewer:v3 . --push
docker run -p 80:80 douguohai/pdfjs-viewer:v3
```

## Usage

```bash
http://localhost:8000/web/viewer.html?file=https://xxx.xxx.com/20230315.pdf
```
