# Usar uma imagem oficial do Python
FROM python:3.10-slim

# Definir diretório de trabalho dentro do contêiner
WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt


# Copiar o código para dentro do contêiner
COPY hello.py .

# Expõe a porta
EXPOSE 8000

# Comando que será executado quando o contêiner iniciar
CMD ["python", "hello.py"]
