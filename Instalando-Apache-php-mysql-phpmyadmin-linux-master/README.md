# Instalando-Apache-php-mysql-phpmyadmin Linux
Instalando APACHE + MYSQL/Phpmyadmin via **Terminal**

Para instalar uma versão do php diferente do que vai encontrar aqui, basta digitar o mesmo comando, apenas alterando o "número" da versão.

Abra seu terminal e execute o comando:

`sudo su`

Esse comando é para dar acesso de administrador(**root**) no terminal.
Assim não será necessário a todo momento inserir o comando sudo e colocar senha.

Comando para REINICIAR o serviço do APACHE, digite no terminal:

`/etc/init.d/apache2 restart`

Instalando o **PHP**

`apt install php7.2 php7.2-mysql`

Instalando o **MySQL**

`apt install mysql-server`

Vai aparecer uma tela para configurar a senha de root do gerenciador de banco de dados, só colocar a senha e depois confirmar e apertar enter para que a instalação seja concluída.

Instalando o **Phpmyadmin**

`apt install phpmyadmin`

Vai começar a instalação, quando aparecer uma tela para escolher o servidor WEB **marque a opção do apache2** e de OK.

`Clique na tecla de espaço para selecionar a opção e pressione Enter`

Próxima tela que vai aparecer **diga que SIM** para configurar a base de dados para o Phpmyadmin.

As outras duas tela que vão ser sugerida são para configurar senha de administrador do banco de dados e do Phpmyadmin, sugiro que coloquem a mesma senha de root do MySQL para que não se confunda com muita senhas.

Ou seja, senha root.

**Dica: reinicialize o serviço do apache depois de tudo instalado.**

Para verificar se o Phpmyadmin esta funcionando direitinho abra o navegador da internet e digite localhost/phpmyadmin na barra de endereço e pressione enter:

**localhost/phpmyadmin**

nesse momento aparecerá a tela de login.
Tente as opções abaixo:

1. **Login: phpmyadmin Senha: root**
2. Login: root Senha: root
3. Login: root Senha:

# Outros tópicos relacionados

>[Recuperar senha do root](https://github.com/marcosviniciusid/Recuperar-senha-de-Root-mysql-phpmyadmin/blob/master/README.md)
>
>[Desinstalar Mysql no linux completamente](https://github.com/marcosviniciusid/Desinstalar-Mysql-no-Linux/blob/master/README.md)
