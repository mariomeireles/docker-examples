# Usa a imagem base oficial do Ubuntu
FROM ubuntu:latest

# Atualiza o sistema e instala o Apache
RUN apt-get update && \
    apt-get install -y apache2 && \
    apt-get clean

# Copia uma página HTML padrão para o servidor (opcional)
RUN echo '<!DOCTYPE html><html><head><meta charset="UTF-8"></head><body><h1>Servidor Apache no Docker</h1><p>Este é um servidor Apache em um contêiner Docker.</p></body></html>' > /var/www/html/index.html

# Expõe a porta 80 para acesso externo
EXPOSE 80

# Inicia o servidor Apache em primeiro plano
CMD ["apachectl", "-D", "FOREGROUND"]
