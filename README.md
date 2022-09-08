# modelagem-oficina
Modelagem Oficina, desenvolvido para Database Experience
<div>
<h3>Objetivo:</h3>
Cria o esquema conceitual para o contexto de oficina com base na narrativa fornecida
<h3>Narrativa:</h3>
<ul>
  <li>	Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica</li>
  <li>	Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões  periódicas</li>
  <li>	Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma OS com data de entrega.</li>
  <li>	A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra</li>
  <li>	O valor de cada peça também irá compor a OSO cliente autoriza a execução dos serviços</li>
  <li>	A mesma equipe avalia e executa os serviços</li>
  <li>	Os mecânicos possuem código, nome, endereço e especialidade</li>
  <li>	Cada OS possui: n°, data de emissão, um valor, status e uma data para conclusão dos trabalhos.</li>
</ul>
</div>

  <h1>Solução:</h1>
  

![Oficina](https://user-images.githubusercontent.com/39250586/189178653-6b01468c-d44e-4d66-b812-83f08737410a.png)

<ul>
    <li>Um cliente tem um ou mais veículos, um veículos pertence a um cliente.</li>
    <li>Um veículo é analisado por um ou mais mecânicos, um mecânico analisa um ou mais veículos.</li>
    <li>Um mecânico Avalia / Executa um ou mais serviços, e um serviço, é avaliado / executado por um ou mais mecânicos.</li>
    <li>Um mecânico preenche uma ou mais OS's, OS é preenchido por um ou mais mecânicos.</li>
    <li>Uma OS tem uma ou mais peças, e uma peça compõe uma ou mais OS's.</li>
    <li>Uma OS tem um ou mais serviços, e um serviço esta em uma ou mais OS's.</li>
    <li>Um cliente autoriza um ou mais OS's, uma OS é autorizada por um cliente.</li>
    <li>Um serviço pode ter um conserto ou uma revisão.</li>
</ul>
