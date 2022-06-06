## MOMENTO & SEUS FUNCIONÁRIOS - BANCO DE DADOS (MySQL)  <img align="center" height="60" width="70" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg">

<h4> ⭐A MOMENTO É UMA EMPRESA ÚNICA QUE FAZ O MELHOR QUE PODE PARA ALCANÇAR O MELHOR DA HUMANIDADE!⭐</h4>

##

<h3> 1 - Inclua suas próprias informações no departamento de tecnologia da empresa. </h3>
<code>INSERT INTO funcionarios (`primeiro_nome`, `sobrenome`, `email`, `telefone`, `dataContratacao`, `ocupacao_id`, `salario`, `departamento_id`) VALUES ('João Vitor','Conrado','JoaoSConrado@gmail.com','4002 8922','2022-06-06',(SELECT ocupacao_id FROM ocupacoes WHERE ocupacao_title LIKE '%Desenvolvedor Web%'),'4000.00',(SELECT departamento_id FROM departamento WHERE departamento_name LIKE '%Tecnologia%')); </code>

##
![1](https://user-images.githubusercontent.com/99970376/172224607-0945e709-9104-45bd-bf7d-0f4b4f4b3a30.PNG)
##

