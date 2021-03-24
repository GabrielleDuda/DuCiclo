# TRABALHO 01:  DuCiclo
Trabalho desenvolvido durante a disciplina de BD1

# Sumário

### 1. COMPONENTES<br>
Integrantes do grupo<br>
Gabrielle Duda: gabiabacduda@gmail.com<br>
Renato Marques: renatomtf26@gmail.com<br>
<br>

### 2.INTRODUÇÃO E MOTIVAÇÃO<br>
> Em meio a toda a crise mundial causada pela pandemia do Coronavírus, muitos lojistas tiveram que reinventar suas vendas presencias para não serem afetados. Segundo a ValorInveste o crescimento no setor de delivery beira 94%, e com isso uma nova oportunidade surge para quem perdeu seu emprego em meio a toda essa situação: trabalhar com entregas de mercadorias. O DuCiclo é um aplicativo que visa ajudar e crescer junto com essa nova onda de superação, interligando pequenos e grandes lojistas de diversos setores com entregadores motivados a ganharem uma nova renda. O sistema proposto é mais que um app de logistica de entrega, a ideia é criar oportunidades! O entregaDu, ao adentrar na plataforma recebe um codnome carinhoso e tambem a chance de trabalhar seja qual for o seu meio de locomoção (carro, moto, bicicleta, patins, cavalo), basta se cadastrar e se empenhar de acordo com sua possibilidade. Um cliente com sua mercadoria, o vendedor com sua venda, e o entregador com sua nova jornada.
 

### 3.MINI-MUNDO<br>

A plataforma DuCiclo têm a ideia de interligar motoboys, lojistas e clientes, com o objetivo de entregar com segurança qualquer coisa que possa ser carregada de maneira segura. A missão da plataforma é resolver o problema de lojistas que agora atendem delivery mas não possuem serviços próprios de entrega de mercadoria, além de gerar empregos para entregadores que não possuam carro ou moto para realizar a entrega.  Primeiramente ocorre um cadastro no aplicativo onde lojista se cadastra com CNPJ ou CPF, nome do estabelecimento ("nome fantasia"), Razão social, nome do responsável, telefone, endereço da loja. Os entregadores podem ser motoboys, ciclistas, ou usuários de qualquer forma de locomoção, desde de que façam acesso a plataforma cadastrando previamente cadastrar nome, cpf, data de nascimento (para que não sejam catalogados menores de idade), meio de transporte, escolhe a área geográfica de atuação,  telefone para contato. A área geográfica vai ajudar a delimitar a atuação do entregador e assim possibilitar maior segurança no prazo para entrega das encomendas, previamente existentes na plataforma essa tem opções de grupos de bairros para atendimento. O cliente tambem pode se cadastrar com nome e telefone, sua função é acompanhar a entrega. O lojista cadastra a encomenda (nome do produto, descrição, valor, quantidade, data da entrega, hora da retirada da entrega) e estas são agrupadas por bairros proximos. O aplicativo apresenta ao entregador, de acordo com sua área, as entregas disponiveis para o dia seguinte, importante salientar que para o sistema de agrupamento de áreas próximas funcione é importante salienar: as entregas tem prazo de 24horas para ocorrer. Em outras palavras, o lojista cadastra mas não serão retiradas da loja no dia de cadastro da entrega. Quando o entregaDu aceita uma encomenda  é criado o pedido, que interliga o cliente cadastrado previamente (importante o logista orientar ao cliente essa necessidade), ao entregaDu e a encomenda cadastrada pelo lojista. Entrega feita então se avalia todos os critérios por todos os envolvidos e assim a plataforma ganha em melhoria de atuação.

### 4.PROTOTIPAÇÃO, PERGUNTAS A SEREM RESPONDIDAS E TABELA DE DADOS<br>
#### 4.1 RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>

![Proposta de logo] <img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/LOGO.jpeg?raw=true" height="200px"><br><br>

![Pasta com possiveis telas](https://github.com/GabrielleDuda/DuCiclo/tree/main/imagens)

<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/modelo%20-%20loggin.png?raw=true" height="300px">


![Arquivo PDF do Protótipo Balsamiq feito para Aplicativo DuCiclo](https://github.com/GabrielleDuda/DuCiclo/blob/main/Prototipo-%20Renato%20Marques%20e%20Gabrielle%20Azevedo.pdf?raw=true "Aplicativo DuCiclo")

#### 4.2 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?
      
> O aplicativo DuCiclo precisa inicialmente dos seguintes relatórios:
* Relatório de entregadores por bairro ou cidade.
* Relatório de compradores por bairro ou cidade.
* Relatorio de entregas por período.
* Relatório de entregadores com mais entregas por período.
* Relatório de lojistas com mais vendas por período.
* Relatório de bairros que mais possuem pedidos de delivery

 
#### 4.3 TABELA DE DADOS DO SISTEMA:
    
![Exemplo de Tabela de dados do Aplicativo DuCiclo](https://github.com/GabrielleDuda/DuCiclo/blob/main/arquivos/TABELA%20DE%20DADOS.xlsx?raw=true "Tabela - Aplicativo DuCiclo")
    
    
### 5.MODELO CONCEITUAL<br>
![Alt text](https://github.com/GabrielleDuda/DuCiclo/blob/main/arquivos/conceitual%20-%20DUCICLO.png?raw=true "Modelo Conceitual")
    
         
    
#### 5.1 Validação do Modelo Conceitual
    [Grupo01]: Claudio Magno e Diogo Tomas : "Achei bem interessante a idéia, principalmente nesse período atual, só não entendi bem onde o endereço do cliente seria armazenado, pois o modelo conceitual do seu projeto apenas o lojista possui o endereço"
    [Grupo02]: Eduardo Alves, Renato Peres e Thiago Corrêa: "Acho q deveria ter o código do lojista na encomenda, e a cardinalidade de encomenda-lojista acho q deveria ser 1,1 do lado do lojista, acho q tinha que ter uma fk para o endereço na tabela do lojista, a cardinalidade de encomenda-cliente acho q deveria ser 1,1 do lado do cliente."
    

#### 5.2 Descrição dos dados 

> LOJISTA: Tabela que armazena as informações relativa a loja que necessita da entrega.

*nomefantasia: campo que armazena o nome popularizado da loja

*CNPJ: campo que armazena o número de identicação da loja de caracter jurídico

*razaosocial: campo que armazena o nome jurídico da loja 

*nome_resp: campo que armazena o nome do funcionário que responde pela loja

*telefone: campo que armazena o número para comunicação com o lojista

*id_lojista: campo que armazena o código de identificação do lojista dentro do aplicativo


> ENTREGADU: Tabela que armazena os dados dos entregadores cadastrados no aplicativo
> 
*cod_entregador: campo que armazena o código de identificação do entregador dentro do aplicativo

*nome: campo que armazena o nome do entregador

*telefone: campo que armazena o telefone do entregador

*meio_transporte: campo que armazena o meio de locomoção do entregador

*data_nascimento: campo que armazena a data de nascimento do entregador

*cpf: campo que armazena o número do CPF do entregador para identificação externa do mesmo


> CLIENTE: Tabela que armazena os dados dos clientes que compraram nas lojas cadastradas e esperam a encomenda

*cod_cliente: campo que armazena o código de identificação do cliente dentro do aplicativo

*nome: campo que armazena o nome do cliente

*telefone: campo que armazena o telefone do cliente


> ENCOMENDA: Tabela que armazena os dados das encomendas feitas pelos lojistas cadastrados no aplicativo

*cod_encomenda: campo que armazena o código que identifica o cliente dentro do aplicativo

*nomeprod: campo que armazena o nome do produto que será entregue 

*descricao: campo que armazena a descrição do contéudo da encomenda

*quantidade: campo que armazena a quantidade de produtos estão sendo tratados dentro da encomenda

*data_entrega: campo que armazena a data que a entrega deve ser levada até o cliente

*hora_retirada: campo que armazena a hora que a encomenda pode ser retirada da loja


> entrega: Tabela que faz a relação entre entregador, cliente e encomenda

> escolhe: Tabela que faz a relação entre os entregadores dentro da mesma área geografica


> ENDERECO: Tabela que armazena informações relativas ao endereço dos cadastrados

*logradouro: campo que armazena o nome da rua, viela, avenida dos cadastrados

*numero: campo que armazena o número da casa dos cadastrados

*bairro: campo que armazena o nome do bairro do cadastrado

*cidade: campo que armazena o nome da cidade do cliente

*cep: campo que armazena o cep para localização externa do cadastrado

*complemento: campo que armazena dados complementares para encontrar o cadastrado

*refencia: campo que armazena um ponto de referencia do endereço do cadastrado


> AREA_GEOGRAFICA: Tabela que armazena informações relativas ao quadro de endereços de uma mesma área

*nome: campo que armazena o nome da area geografica agrupada

*cidade: campo que armazena as cidades dentro da área georgráfica

*bairro: campo que armazena o nome do bairros dentro da área georgráfica


### 6	MODELO LÓGICO<br>

![Modelo Lógico - DuCiclo](https://github.com/GabrielleDuda/DuCiclo/blob/main/arquivos/logico%20-%20DUCICLO.png?raw=true "Modelo LÓGICO")


### 7	MODELO FÍSICO<br>

CREATE TABLE LOJISTA (nomefantasia varchar(50), CNPJ char(13), razaosocial varchar(50), nome_resp varchar(50), telefone char(11), id_lojista integer PRIMARY KEY);

CREATE TABLE ENTREGADU (cod_entregador integer PRIMARY KEY, nome varchar(50), telefone char(11), area_geografica varchar(30), meio_transporte varchar(50), data_nascimento date, cpf char(11);

CREATE TABLE CLIENTE (cod_cliente integer PRIMARY KEY, nome varchar(50), telefone varchar(11));

CREATE TABLE ENCOMENDA (cod_encomenda integer PRIMARY KEY, nomeprod varchar(50), descricao varchar(50), quantidade int, data_entrega date, hora_retirada timestamp, FK_LOJISTA integer,  FOREIGN KEY (FK_LOJISTA) REFERENCES LOJISTA (id_lojista), FK_CLIENTE);

CREATE TABLE ENDERECO (logradouro varchar(50), número int, bairro varchar(50), cep char(8), cidade varchar(50), complemento varchar(50), refencia varchar(50), cod_lojista integer, id_cliente integer, FOREIGN KEY (cod_lojista) REFERENCES LOJISTA (id_lojista), FOREIGN KEY (id_cliente) REFERENCES CLIENTE (cod_cliente));

CREATE TABLE PEDIDO(fk_encomenda integer, cod_pedido integer PRIMARY KEY, fk_ENTREGADU integer, fk_CLIENTE integer, FOREIGN KEY (fk_ENTREGADU) REFERENCES ENTREGADU (cod_entregador), FOREIGN KEY (fk_CLIENTE) REFERENCES CLIENTE (cod_cliente), FOREIGN KEY (fk_encomenda) REFERENCES ENCOMENDA (cod_encomenda));



       
       
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>



### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
    
    
    
    
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>





># Marco de Entrega 01: Do item 1 até o item 9.1<br>

#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>
#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not
    b) Criar no mínimo 3 consultas com operadores aritméticos 
    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas

#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.

#### 9.5	INSTRUÇÕES APLICANDO ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>
    a) Criar minimo 3 de exclusão
    b) Criar minimo 3 de atualização

#### 9.6	CONSULTAS COM INNER JOIN E ORDER BY (Mínimo 6)<br>
    a) Uma junção que envolva todas as tabelas possuindo no mínimo 2 registros no resultado
    b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho

#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>
    a) Criar minimo 2 envolvendo algum tipo de junção

#### 9.8	CONSULTAS COM LEFT, RIGHT E FULL JOIN (Mínimo 4)<br>
    a) Criar minimo 1 de cada tipo

#### 9.9	CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)<br>
        a) Uma junção que envolva Self Join (caso não ocorra na base justificar e substituir por uma view)
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho

#### 9.10	SUBCONSULTAS (Mínimo 4)<br>
     a) Criar minimo 1 envolvendo GROUP BY
     b) Criar minimo 1 envolvendo algum tipo de junção

># Marco de Entrega 02: Do item 9.2 até o ítem 9.10<br>

### 10 RELATÓRIOS E GRÁFICOS

#### a) análises e resultados provenientes do banco de dados desenvolvido (usar modelo disponível)
#### b) link com exemplo de relatórios será disponiblizado pelo professor no AVA
#### OBS: Esta é uma atividade de grande relevância no contexto do trabalho. Mantenha o foco nos 5 principais relatórios/resultados visando obter o melhor resultado possível.

    

### 11	AJUSTES DA DOCUMENTAÇÃO, CRIAÇÃO DOS SLIDES E VÍDEO PARA APRESENTAÇAO FINAL <br>

#### a) Modelo (pecha kucha)<br>
#### b) Tempo de apresentação 6:40 

># Marco de Entrega 03: Itens 10 e 11<br>
<br>
<br>
<br> 




