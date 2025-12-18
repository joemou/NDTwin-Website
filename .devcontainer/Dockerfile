# 使用輕量級的 Node.js 環境 (Debian based)
FROM mcr.microsoft.com/devcontainers/javascript-node:18

# 手動下載並安裝 Hugo Extended v0.121.1 (指定這個穩定版本，保證有檔案)
RUN wget -q -O hugo.tar.gz https://github.com/gohugoio/hugo/releases/download/v0.121.1/hugo_extended_0.121.1_linux-amd64.tar.gz \
    && tar -xf hugo.tar.gz \
    && mv hugo /usr/local/bin/hugo \
    && rm hugo.tar.gz \
    && echo "Hugo installed successfully!"