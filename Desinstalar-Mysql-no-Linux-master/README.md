# Desinstalar-Mysql-no-Linux

Desinstalando Mysql no Linux por completo.

Primeiro passo é verificar se está instalado o programa com o seguinte comando:

`dpkg -l mysql-server`

Como podemos ver o resultado do comando, o pacote esta com "ii" no começo da linha, significa que o pacote está instalado.

`sudo apt-get remove --purge mysql-server`

Próximo passo remover o PHPMYADMIN - gerenciador gráfico de banco de dados.

`sudo apt-get remove --purge phpmyadmin `

Vai aparecer duas telas a seguir selecione a opção sim quando elas aparecerem vai pedir a senha do administrador do banco coloque a senha e confirme.

# Vamos parar o serviço do MySQL.

`sudo /etc/init.d/mysql stop`

Agora vamos remover mais um pacote do MySQL.

`sudo apt-get remove --purge mysql-common`


Por ultimo apague a pasta mysql que fica localizada em /var/lib/ com o comando abaixo e pressione enter:

`sudo rm -rf /var/lib/mysql`

Depois de fazer todos os passos acima digite um comando de cada vez no terminal:

1. `sudo apt-get autoremove --purge`
2. `sudo apt-get autoclean`
3. `sudo apt-get clean`

Reiniciar o mysql

`/etc/init.d/mysql restart`

Finalizado.

# Outros tópicos

>[Instalando Apache + php + Mysql + phpmyadmin](https://github.com/marcosviniciusid/Linux/tree/master/Instalando-Apache-php-mysql-phpmyadmin-linux-master)
>
>[Recuperar senha do root](https://github.com/marcosviniciusid/Linux/tree/master/Recuperar-senha-de-Root-mysql-phpmyadmin-master)
