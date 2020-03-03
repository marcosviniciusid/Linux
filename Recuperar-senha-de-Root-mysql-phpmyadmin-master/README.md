# Recuperar-senha-de-Root-mysql-phpmyadmin
Recuperar senha de root do phpmyadmin. Do erro: **mysqli_real_connect(): (HY000/1698): Access denied for user 'root'@'localhost'**

Abra seu terminal e execute os comandos abaixo:

1. `mysql -u root -p`
2. `CREAT USER 'admin'@'%' IDENTIFIED BY 'admin4321';`
3. `GRANT ALL PRIVILEGES ON *.* TO 'admin'@'%' WITH GRANT OPTION;`

Após isso, acesso o localhost/phpmyadmin e logue com o novo usuário.

`admin | admin4321`

Após isso, poderá alterar a senha do root na aba de '*Contas de usuários*'.


# Outros tópicos

>[Desinstalar Mysql no linux completamente](https://github.com/marcosviniciusid/Linux/tree/master/Desinstalar-Mysql-no-Linux-master)
>
>[Instalando APACHE + MYSQL/Phpmyadmin via **Terminal**](https://github.com/marcosviniciusid/Linux/tree/master/Instalando-Apache-php-mysql-phpmyadmin-linux-master)
