World Time API é um serviço web simples que retorna a hora local atual para um determinado fuso horário como texto simples ou JSON.
https://worldtimeapi.org

Código JavaScript, Thymeleaf, e CSS para consumir a API WorldTimeAPI e preencher campos de entrada com os dados retornados ao selecionar um timezone na combobox.

Detalhes do código
------------------
O HTML exibe um combobox com a lista de timezones e campos de entrada para exibir os dados automaticamente.

O JavaScript adiciona um evento ao combobox que, ao selecionar um timezone, envia uma requisição fetch à API. Os dados retornados são preenchidos nos 
campos de entrada.
O CSS estiliza os campos de forma simples.

Carregamento dos Timezones:
---------------------------
O fetch chama o endpoint https://worldtimeapi.org/api/timezone para obter a lista de timezones e, para cada timezone recebido, cria um novo <option> no COMBOBOX.

Seleção de Timezone:
--------------------
O script escuta mudanças no COMBOBOX e faz uma segunda requisição para a API para obter os detalhes daquele timezone específico.
Isso garantirá que os timezones apareçam no COMBOBOX ao carregar a página.
