# Use a imagem oficial do PHP
FROM php:8.0-apache

# Define o diretório de trabalho dentro do contêiner
WORKDIR /var/www/html

# Instala as extensões PHP necessárias
RUN docker-php-ext-install pdo pdo_mysql

# Copia os arquivos do aplicativo Laravel para o contêiner
COPY . /var/www/html

# Habilita o módulo rewrite do Apache
RUN a2enmod rewrite

# Define as permissões adequadas
RUN chown -R www-data:www-data /var/www/html/storage /var/www/html/bootstrap/cache

# Expõe a porta 80 para o tráfego da web
EXPOSE 80

# Comando para iniciar o Apache em primeiro plano
CMD ["apache2-foreground"]
