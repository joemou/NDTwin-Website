# 使用輕量級的 Node.js 環境
FROM mcr.microsoft.com/devcontainers/javascript-node:18

# 1. 安裝必要工具和 Go 語言
RUN apt-get update && apt-get install -y golang-go curl wget

# 2. 自動抓取 Github 上 "最新版" 的 Hugo Extended
# 這樣我們就不用一直手動改版號，保證符合 Docsy 的最新需求
RUN version=$(curl -s https://api.github.com/repos/gohugoio/hugo/releases/latest | grep tag_name | cut -d '"' -f 4 | cut -c 2-) \
    && echo "Downloading Hugo version: $version" \
    && wget -q -O hugo.tar.gz "https://github.com/gohugoio/hugo/releases/download/v${version}/hugo_extended_${version}_linux-amd64.tar.gz" \
    && tar -xf hugo.tar.gz \
    && mv hugo /usr/local/bin/hugo \
    && rm hugo.tar.gz \
    && hugo version

# 3. 驗證安裝是否成功
RUN echo "Hugo installation complete!"