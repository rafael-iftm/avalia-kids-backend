# Usa a imagem oficial do OpenJDK 17
FROM openjdk:17-jdk-slim

# Define o diretório de trabalho dentro do container
WORKDIR /app

# Copia o JAR gerado pelo Maven para dentro do container
COPY target/eureka-server-0.0.1-SNAPSHOT.jar app.jar

# Expõe a porta que o serviço irá rodar
EXPOSE 8761

# Comando para rodar o serviço dentro do container
ENTRYPOINT ["java", "-jar", "app.jar"]
