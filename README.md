# desafio-e-Commerce
Criação de esquema conceitual de banco de dados 

Foi criado uma entidade Cliente e uma entidade veículo separadamente pois um mesmo cliente poderia ter vários veículos, 
já o relacionamento com a OS é com o veículo, e a aprovação é feita pelo cliente, o status TINYINT possibilitaria receber
valores de -128 a 127, o que poderia ter uma tabela em separado para discriminar qual seria o status correspondente 
(observação incluída no arquivo do MySQL workbench, onde o status da OS poderá ser por exemplo: 1-Em elaboração; 2-Em aprovação;
3-Aprovada; 4-Encerrada (esta poderia ser considerada tanto quando o serviço for terminado quanto quando estiver devidamente paga
pelo cliente.
entidades intermediárias foram representadas para indicar o relacionamento (Cliente_has_OS; veículo_ha_OS; OS_has_Peças; OS_has_Serviço)
e a possibilidade de um Cliente ter um ou mais veículos está indicada no tipo de relacionamento 1-n.
