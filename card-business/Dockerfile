# qual imagem será utilizada
FROM ubuntu:22.04

# criando container
RUN apt-get update && apt-get install -y python3.11 python3.11-dev python3-pip

# criar a pasta que vai ser containerizada
WORKDIR /app

# copiar de . para /app (dentro do ubuntu)
COPY . /app

# executando dentro do container
RUN pip3 install --no-cache-dir -r requirements.txt

# qual porta a aplicação está rodando
EXPOSE 8080

# definir variáveis de ambiente (se o projeto precisar)
ENV LOGOMARCA="https://imgs.search.brave.com/UdlHSCJEJn4dLPiiK8OQFXsFsQp0zvMa2jBKEbYJlrI/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9ia3Qt/c2EtZWFzdC0xLWNt/cy1kcnVwYWwuczMt/c2EtZWFzdC0xLmFt/YXpvbmF3cy5jb20v/Y21zL2FsZGEucG5n"
ENV FOTO="https://imgs.search.brave.com/VkLMsFTyCtmM4_5TrX5nYmUflAXeBUNLXBSH3DuAAS8/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly91cGxv/YWQud2lraW1lZGlh/Lm9yZy93aWtpcGVk/aWEvY29tbW9ucy9i/L2I2L0ltYWdlX2Ny/ZWF0ZWRfd2l0aF9h/X21vYmlsZV9waG9u/ZS5wbmc"
ENV NOME="Matias"
ENV IDADE="18"
ENV EMAIL="maitas@email.com"
ENV PROFISSAO="Programador Freelancer"
ENV SITE="github.com/Matiaszz"

CMD ["python3", "app.py"]
