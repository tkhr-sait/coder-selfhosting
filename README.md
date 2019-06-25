# coder-selfhosting

## Play With Docker

### 遊び方

0. Dockerアカウント登録 https://hub.docker.com/
1. https://labs.play-with-docker.com/
2. Login -> Start -> +ADD NEW INSTANCE
3. curl -O https://raw.githubusercontent.com/tkhr-sait/coder-selfhosting/master/pwd/docker-compose.yml
4. docker-compose up -d
5. PWD上部に出てきた 8443 のリンク
6. 遊んでみる ※SSL/パスワード設定などしていないので、パスワード/TOKENなど重要な情報は入れないように！

### ビルド 

0. git clone https://github.com/tkhr-sait/coder-selfhosting
1. cd coder-selfhosting/pwd
2. docker build -t tkhr0sait/code-server-custom:latest -f Dockerfile.code-server .
3. docker login
4. docker push tkhr0sait/code-server-custom:latest