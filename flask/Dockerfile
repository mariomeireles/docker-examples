# Use uma imagem base oficial do Python
FROM python:3.8-slim

# Defina o diretório de trabalho
WORKDIR /app

# Copie os arquivos necessários para o conteiner
COPY . /app

# Instale as dependências
RUN pip install Flask

# Exponha a porta em que o Flask está rodando
EXPOSE 5000

# Comando para rodar a aplicação
CMD ["python", "app.py"]
