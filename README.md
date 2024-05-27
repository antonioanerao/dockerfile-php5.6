### Docker Image para projetos com PHP 5.6 e MySQL 5.7.44

#### Apache
    2.4.25

#### PHP
    5.6.40

#### Extensões PHP
    Core
    ctype
    curl
    date
    dom
    ereg
    fileinfo
    filter
    ftp
    gd
    hash
    iconv
    json
    libxml
    mbstring
    mhash
    mysql
    mysqlnd
    openssl
    pcre
    PDO
    pdo_mysql
    pdo_sqlite
    Phar
    posix
    readline
    Reflection
    session
    SimpleXML
    SPL
    sqlite3
    standard
    tokenizer
    xml
    xmlreader
    xmlwriter
    zlib

#### Pasta root dentro do container
    /var/www/html

### Como rodar

#### Clonar este repo
    $ git clone https://github.com/antonioanerao/dockerfile-php5.6.git

#### Acessa a pasta do repo
    $ cd dockerfile-php5.6

#### Build da imagem
    $ docker build -t php5.6 .

#### Crie uma rede docker chamada proxy
    $ docker network create proxy

#### Suba a aplicação
    $ docker compose -f dev.yml up -d

A aplicação ficará disponível no endereço encontrado no dev.yml, que é _http://webserver.docker.localhost_
