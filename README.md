## MOMENTO & SEUS FUNCIONÁRIOS - BANCO DE DADOS (MySQL)  <img align="center" height="60" width="70" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg">

<h4> ⭐A MOMENTO É UMA EMPRESA ÚNICA QUE FAZ O MELHOR QUE PODE PARA ALCANÇAR O MELHOR DA HUMANIDADE!⭐</h4>

##

<h3> 1 - Inclua suas próprias informações no departamento de tecnologia da empresa. </h3>
<code>INSERT INTO funcionarios (`primeiro_nome`, `sobrenome`, `email`, `telefone`, `dataContratacao`, `ocupacao_id`, `salario`, `departamento_id`) VALUES ('João Vitor','Conrado','JoaoSConrado@gmail.com','4002 8922','2022-06-06',(SELECT ocupacao_id FROM ocupacoes WHERE ocupacao_title LIKE '%Desenvolvedor Web%'),'4000.00',(SELECT departamento_id FROM departamento WHERE departamento_name LIKE '%Tecnologia%')); </code>

##
![1](https://user-images.githubusercontent.com/99970376/172224607-0945e709-9104-45bd-bf7d-0f4b4f4b3a30.PNG)
##

<h3> 2 -  A administração está sem funcionários. Inclua os outros elementos do seu grupo do demoday no departamento de administração. </h3>

<code> INSERT INTO funcionarios (`primeiro_nome`, `sobrenome`, `email`, `telefone`, `dataContratacao`, `ocupacao_id`, `salario`, `departamento_id`) VALUES ('Larissa','Pereira','LarissaPereira1010@gmail.com','4003 8922','2022-06-06',(SELECT ocupacao_id FROM ocupacoes WHERE ocupacao_title LIKE '%Assistente Administrativo%'),'3000.00',(SELECT departamento_id FROM departamento WHERE departamento_name LIKE '%Admnistração%')); </code>

<code> INSERT INTO funcionarios (`primeiro_nome`, `sobrenome`, `email`, `telefone`, `dataContratacao`, `ocupacao_id`, `salario`, `departamento_id`) VALUES ('Lara','Rufino','LaraRufino2020@gmail.com','4004 8922','2022-06-06',(SELECT ocupacao_id FROM ocupacoes WHERE ocupacao_title LIKE '%Assistente Administrativo%'),'3000.00',(SELECT departamento_id FROM departamento WHERE departamento_name LIKE '%Admnistração%')); </code>

<code> INSERT INTO funcionarios (`primeiro_nome`, `sobrenome`, `email`, `telefone`, `dataContratacao`, `ocupacao_id`, `salario`, `departamento_id`) VALUES ('Luana','Andrade','LuanaAndrade3030@gmail.com','4005 8922','2022-06-06',(SELECT ocupacao_id FROM ocupacoes WHERE ocupacao_title LIKE '%Assistente Administrativo%'),'3000.00',(SELECT departamento_id FROM departamento WHERE departamento_name LIKE '%Admnistração%')); </code>

<code> INSERT INTO funcionarios (`primeiro_nome`, `sobrenome`, `email`, `telefone`, `dataContratacao`, `ocupacao_id`, `salario`, `departamento_id`) VALUES ('Andre','Palhares','AndrePalhares10@gmail.com','2022 8922','2022-06-06',(SELECT ocupacao_id FROM ocupacoes WHERE ocupacao_title LIKE '%Assistente Administrativo%'),'3000.00',(SELECT departamento_id FROM departamento WHERE departamento_name LIKE '%Admnistração%')); </code>

<code> INSERT INTO funcionarios (`primeiro_nome`, `sobrenome`, `email`, `telefone`, `dataContratacao`, `ocupacao_id`, `salario`, `departamento_id`) VALUES ('Eduardo','Oliveira','EduardoOliveira9090@gmail.com','4012 8922','2022-06-06',(SELECT ocupacao_id FROM ocupacoes WHERE ocupacao_title LIKE '%Assistente Administrativo%'),'3000.00',(SELECT departamento_id FROM departamento WHERE departamento_name LIKE '%Admnistração%')); </code>

<code> INSERT INTO funcionarios (`primeiro_nome`, `sobrenome`, `email`, `telefone`, `dataContratacao`, `ocupacao_id`, `salario`, `departamento_id`) VALUES ('Mayara','Rodrigues','MayaraRodrigues7070@gmail.com','4009 8922','2022-06-06',(SELECT ocupacao_id FROM ocupacoes WHERE ocupacao_title LIKE '%Assistente Administrativo%'),'3000.00',(SELECT departamento_id FROM departamento WHERE departamento_name LIKE '%Admnistração%')); </code>

<code> INSERT INTO funcionarios (`primeiro_nome`, `sobrenome`, `email`, `telefone`, `dataContratacao`, `ocupacao_id`, `salario`, `departamento_id`) VALUES ('Nicolly','Gabrielly','NicollyGabrielly5050@gmail.com','4007 8922','2022-06-06',(SELECT ocupacao_id FROM ocupacoes WHERE ocupacao_title LIKE '%Assistente Administrativo%'),'3000.00',(SELECT departamento_id FROM departamento WHERE departamento_name LIKE '%Admnistração%')); </code>

##
![2](https://user-images.githubusercontent.com/99970376/172229630-6d762fa5-a263-4175-8d60-9283b8a87daf.PNG)
##

<h3> 3 -  Agora diga, quantos funcionários temos ao total na empresa? </h3>
Na empresa tem 48 funcionários! <code> SELECT COUNT(*) FROM funcionarios; </code>

##
![3](https://user-images.githubusercontent.com/99970376/172230091-6e99acdd-8bfa-48f6-85d5-0f339a62fc23.PNG)
##

<h3> 4 -  Quantos funcionários temos no departamento de finanças? </h3>
Na empresa tem 48 funcionários do departamento de finanças! <code> SELECT COUNT(*) FROM funcionarios WHERE departamento_id LIKE '%10%' </code>

##
![4](https://user-images.githubusercontent.com/99970376/172230938-c2cded06-e720-4dcb-8caf-4719bab50158.PNG)
##

<h3> 5 -  Qual a média salarial do departamento de tecnologia? </h3>
A média salarial é de: R$: 5467,00! <code> SELECT ROUND(AVG(salario)) from funcionarios WHERE departamento_id LIKE '%6%' </code>

##
![5](https://user-images.githubusercontent.com/99970376/172232457-e7d0df05-c0d6-40a8-aa12-edc9fed8b810.PNG)
##

<h3> 6 - Quanto o departamento de Transportes gasta em salários? </h3>
Ele gasta: R$ 41200,00! <code> SELECT SUM(salario) from funcionarios WHERE departamento_id LIKE '%5%' </code>

##
![6](https://user-images.githubusercontent.com/99970376/172233229-d947419a-088a-4872-ba77-60918e056f63.PNG)
##

<h3> 7 -   Um novo departamento foi criado. O departamento de inovações. Ele será locado no Brasil. Por favor, adicione-o no banco de dados. </h3>
<code> INSERT INTO `departamento`(`departamento_id`, `departamento_name`, `posicao_id`) VALUES ('','Inovações','5400') </code>

##
![7](https://user-images.githubusercontent.com/99970376/172234139-b354e37c-e90d-48b3-8355-831d8eb8f912.PNG)
##

<h3> 8 -  Novos Funcionários! </h3>
Três novos funcionários foram contratados para o departamento de inovações. Por favor, adicione-os: William Ferreira, casado com Inara Ferreira, possui um filho chamado Gabriel que tem 4 anos e adora brincar com cachorros. Ele será programador.Já a Fernanda Lima, que é casada com o Rodrigo, não possui filhos. Ela vai ocupar a posição de desenvolvedora.  Por último, a Gerente do departamento será Fabiana Raulino. Casada, duas filhas (Maya e Laura). 
O salário de todos eles será a média salarial dos departamentos de administração e finanças. 

<h4> Inserção dos Funcionários: </h4>

<code> INSERT INTO funcionarios (`primeiro_nome`, `sobrenome`, `email`, `telefone`, `dataContratacao`, `ocupacao_id`, `salario`, `departamento_id`) VALUES ('William','Ferreira','WillFerreira01@gmail.com','4002 8923','2022-06-08',(SELECT ocupacao_id from ocupacoes WHERE ocupacao_title LIKE '%Desenvolvedor Web%'),'',(SELECT departamento_id from departamento WHERE departamento_name LIKE '%Inovações%'));</code>

<code> INSERT INTO funcionarios (`primeiro_nome`, `sobrenome`, `email`, `telefone`, `dataContratacao`, `ocupacao_id`, `salario`, `departamento_id`) VALUES ('Fernanda','Lima','FernandaLima02@gmail.com','4002 8924','2022-06-08',(SELECT ocupacao_id from ocupacoes WHERE ocupacao_title LIKE '%Desenvolvedor Web%'),'',(SELECT departamento_id from departamento WHERE departamento_name LIKE '%Inovações%'));</code>

<code> INSERT INTO funcionarios (`primeiro_nome`, `sobrenome`, `email`, `telefone`, `dataContratacao`, `ocupacao_id`, `salario`, `departamento_id`) VALUES ('Fabiana','Raulino','FabiGerente@gmail.com','0800 7777','2022-06-08',(SELECT ocupacao_id from ocupacoes WHERE ocupacao_title LIKE '%Gerente de Marketing%'),'',(SELECT departamento_id from departamento WHERE departamento_name LIKE '%Inovações%')); </code>

##
![8a](https://user-images.githubusercontent.com/99970376/172678724-0cd4dec4-43a0-414c-acf5-814cc9b08b48.PNG)
##

<h4> Inserção dos Salários: </h4>

<code> UPDATE `funcionarios` SET `salario`=(SELECT ROUND(AVG(salario)) FROM funcionarios WHERE departamento_id = 10 OR departamento_id = 1) WHERE departamento_id = 12;
</code>

##
![8b](https://user-images.githubusercontent.com/99970376/172679767-e16610f5-02cf-4e69-a248-5af515fb9eec.PNG)
##

<h4> Inserção dos Dependentes: </h4>

<code> INSERT INTO `dependentes`(`dependente_id`, `primeiro_nome`, `sobrenome`, `parentesco`, `funcionario_id`) VALUES ('','Inara','Ferreira','Cônjuge',(SELECT funcionario_id from funcionarios WHERE primeiro_nome LIKE '%William%' AND sobrenome LIKE '%Ferreira%')); </code>

<code> INSERT INTO `dependentes`(`dependente_id`, `primeiro_nome`, `sobrenome`, `parentesco`, `funcionario_id`) VALUES ('','Rodrigo','Lima','Cônjuge',(SELECT funcionario_id from funcionarios WHERE primeiro_nome LIKE '%Fernanda%' AND sobrenome LIKE '%Lima%')); </code> 

<code> INSERT INTO `dependentes`(`dependente_id`, `primeiro_nome`, `sobrenome`, `parentesco`, `funcionario_id`) VALUES ('','Zé','Raulino','Cônjuge',(SELECT funcionario_id from funcionarios WHERE primeiro_nome LIKE '%Fabiana%' AND sobrenome LIKE '%Raulino%')); </code>
  
<code> INSERT INTO `dependentes`(`dependente_id`, `primeiro_nome`, `sobrenome`, `parentesco`, `funcionario_id`) VALUES ('','Gabriel','Ferreira','Filho(a)',(SELECT funcionario_id from funcionarios WHERE primeiro_nome LIKE '%William%' AND sobrenome LIKE '%Ferreira%')); </code>

<code> INSERT INTO `dependentes`(`dependente_id`, `primeiro_nome`, `sobrenome`, `parentesco`, `funcionario_id`) VALUES ('','Maya','Raulino','Filho(a)',(SELECT funcionario_id from funcionarios WHERE primeiro_nome LIKE '%Fabiana%' AND sobrenome LIKE '%Raulino%')); </code>

<code> INSERT INTO `dependentes`(`dependente_id`, `primeiro_nome`, `sobrenome`, `parentesco`, `funcionario_id`) VALUES ('','Laura','Raulino','Filho(a)',(SELECT funcionario_id from funcionarios WHERE primeiro_nome LIKE '%Fabiana%' AND sobrenome LIKE '%Raulino%')); </code>

##
![8c](https://user-images.githubusercontent.com/99970376/172684087-d3620752-c74c-444a-b19e-4cd7795e6b3c.PNG)
##

<h3> 9 -  Informe todas as regiões em que a empresa atua acompanhadas de seus países. </h3>
<code> </code>

##

##

<h3> 10 -  Joe Sciarra é filho de quem? </h3>
<code> </code>

##

##

<h3> 11 -  Jose Manuel possui filhos? </h3>
<code> </code>

##

##

<h3> 12 -  Qual região possui mais países? </h3>
<code> </code>

##

##

<h3> 13 - Exiba o nome cada funcionário acompanhado de seus dependentes. </h3>
<code> </code>

##

##

<h3> 14 -  Karen Partners possui um cônjuge? </h3>
<code> </code>

##

##

<h3> 15 -  O ID da tabela de países não segue um padrão numérico. Na sua visão, qual o impacto disso no desenvolvimento do banco? </h3>
<code> </code>

##

##

<h3> 16 -  Escolha um país para se mudar. Qual seria esse país? Por que escolheria esse país? E o departamento. O que seria? Como seriam seus funcionários? </h3>
<code> </code>

##

##

<h3> 17 -  Atualize as informações na tabela para que seu departamento seja criado. </h3>
<code> </code>

##

##

