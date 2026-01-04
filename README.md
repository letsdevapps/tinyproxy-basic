# Tinyproxy Basic

## Instalação Ubuntu

    sudo apt-get install tinyproxy -y

## Verificar Status atual

    sudo systemctl status tinyproxy

## Rodar/Para no momento

    sudo systemctl start ttinyproxy
    
    sudo systemctl stop ttinyproxy

## Habilitar/Desabilitar durante inicialização

    sudo systemctl enable tinyproxy
    
    sudo systemctl disable tinyproxy

## Configurar Rede ou Browser

Configure sua rede ou browser para HTTP/HTTPS 127.0.0.1:8888

Tinyproxy roda por padrão na porta 8888

Para alterar acesse o arquivo de configuração e procure Port 8888

    sudo nano /etc/tinyproxy/tinyproxy.conf

### Abra o log para acompanhar uso

    sudo tail -f /var/log/tinyproxy/tinyproxy.log

### Teste via terminal console

    curl -x http://127.0.0.1:8888 http://www.exemplo.com

