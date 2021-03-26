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

![Proposta de logo]
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/LOGO.jpeg?raw=true" height="200px"><br><br>

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


CREATE TABLE Area_geografica (
    id_area integer PRIMARY KEY, nome varchar(100), cidade varchar(100), bairro varchar(100) );

CREATE TABLE ENDERECO (
    id_endereco integer PRIMARY KEY, loragradouro varchar(100), numero char(5), bairro varchar(100), cidade varchar(100), cep char(11), complemento varchar(100), referencia varchar(100), id_area integer, FOREIGN KEY (id_area) REFERENCES Area_geografica (id_area) ON DELETE RESTRICT );

CREATE TABLE LOJISTA (
	id_lojista integer PRIMARY KEY, nomefantasia varchar(100), CNPJ char(11), razaosocial varchar(100), nome_resp varchar(100), telefone char(11), id_endereco integer, FOREIGN KEY (id_endereco) REFERENCES ENDERECO (id_endereco) ON DELETE RESTRICT );

CREATE TABLE ENTREGADU (
    cod_entregador integer PRIMARY KEY, nome varchar(100), telefone char(11), meio_transporte varchar(100), data_nascimento date, cpf char(11) );

CREATE TABLE CLIENTE ( 
    cod_cliente integer PRIMARY KEY, nome varchar(100), telefone varchar(11) );

CREATE TABLE ENCOMENDA (
    cod_encomenda integer PRIMARY KEY, nomeprod varchar(50),
    descricao varchar(100), quantidade int, data_entrega date, hora_retirada time,
    cod_cliente integer, id_lojista integer, id_endereco integer,    
	FOREIGN KEY (cod_cliente) REFERENCES CLIENTE (cod_cliente) ON DELETE RESTRICT,
	FOREIGN KEY (id_lojista) REFERENCES LOJISTA (id_lojista) ON DELETE RESTRICT,
	FOREIGN KEY (id_endereco) REFERENCES ENDERECO (id_endereco) ON DELETE RESTRICT
);

CREATE TABLE escolhe (
	id_area integer, cod_entregador integer,
   FOREIGN KEY (cod_entregador) REFERENCES ENTREGADU (cod_entregador) ON DELETE SET NULL
);

CREATE TABLE entrega (
    cod_entregador integer, cod_encomenda integer,
    FOREIGN KEY (cod_entregador) REFERENCES ENTREGADU (cod_entregador) ON DELETE RESTRICT,
    FOREIGN KEY (cod_encomenda) REFERENCES ENCOMENDA (cod_encomenda) ON DELETE SET NULL
);
 

 

       
       
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>

>> insert into Area_geografica (id_area, nome, cidade, bairro ) values (1001,	'AREA01', 'VITORIA', 'Bento Ferreira, Jucutuquara'), (1002, 'AREA02', 'VITORIA', 'Jardim Camburi, Praia do Canto, Goiabeiras'), (1003, 'AREA03', 'SERRA', 'Laranjeiras, Helio Ferraz'), (1004, 'AREA04', 'SERRA', 'Bairro de Fatima'), (1005, 'AREA05', 'VILA VELHA', 'Itapua, Itaparica'), (1006, 'AREA06', 'CARIACICA', 'Campo Grande');

>> insert into ENDERECO (id_endereco, loragradouro, numero, bairro, cidade, cep, complemento, referencia, id_area) values (10,	'Rua 1D', 135, 'Larajeiras', 'Serra', '29160734', 'Predio numero 101', 'Atras da quadra', 1003), (11, 'Rua João Avelange', 445, 'Bairro de Fatima', 'Serra', '29145733', '', 'Perto do posto', 1004), (12, 'Av. Jose Rato', 1001, 'Bairro de Fatima', 'Serra', '29345722', '', 'Perto do shopping', 1004), (13, 'Rua 3R', 112, 'Itapua', 'Vila Velha', '29133987', 'Casa Vermelha', 'Ao lado do bobs', 1005), (14, 'Rua Quintino Denadai', 247, 'Helio Ferraz', 'Serra', '29134113', 'Predio Branco e verde', 'Atras da Escola', 1003), (15, 'Av. Vitoria', 120, 'Bento Ferreira', 'Vitoria', '29198567', '', 'Em frente a Faculdade', 1001), (16, 'Rua Rio Amazonas', 2311, 'Jucutuquara', 'Vitoria', '29188235', '', 'Atras da Praia', 1001), (17, 'Rua Araceli', 1252, 'Campo Grande', 'Cariacica', '29160735', '', 'Depois da Ponte', 1006), (18, 'Rua Jose Antonio Moraes', 135, 'Larajeiras', 'Serra', '29145734', 'Predio numero 201', '', 1003), (19, 'Avenida Alberto Ribeiro', 445, 'Bairro de Fatima', 'Serra', '29345723', '', 'Perto do posto', 1004), (20, 'Rua Dois', 1001, 'Bairro de Fatima', 'Serra', '29133988', '', 'Perto do shopping', 1004), (21, 'Avenida Curitiba', 112, 'Itaparica', 'Vila Velha', '29134114', 'Casa Vermelha', 'Ao lado do bobs', 1005), (22, 'Travessa das flores', 247, 'Helio Ferraz', 'Serra', '29198568', 'Predio Branco e verde', 'Atras da Escola', 1003), (23, 'rua Dr João Andrade', 120, 'Bento Ferreira', 'Vitoria', '29188236', '', 'Em frente a Faculdade', 1001), (24, 'Rua Pintorama', 2311, 'Jucutuquara', 'Vitoria', '29160736', '', 'Atras da Praia', 1001), (25, 'Avenida Dante Michelini', 1252, 'Jardim Camburi', 'Vitoria', '29145735', '', 'Depois da Ponte', 1002), (26, 'Rua Chapot Presvot', 434, 'Praia do Canto', 'Vitoria', '29445724', 'apt 202', 'ed costa vistoria', 1002), (27, 'Travessa Heitor dias', 1002, 'Jardim Camburi', 'Vitoria', '29133989', 'casa', 'esquina com açai dos sabores', 1002), (28, 'Avenia Dr Rui Barros', 22, 'Goiabeiras', 'Vitoria', '29134115', 'apt 1002', 'ed acacio', 1002);

>> insert into LOJISTA (id_lojista, nomefantasia, CNPJ, razaosocial, nome_resp, telefone, id_endereco) values (2544, 'Pastel do Alex', '146295740000162', 'Renan S. Sartorio ME', 'Renan Soares Sartorio', '27916489685', 10), (2545, 'Dujour', '471963234000171', 'Bef Moda Feminina e vestuário', 'Barbara Ferreira', '2792447354', 11), (2546, 'Sapataria do Futuro', '240288106000134', 'Patricia P. de Paulo MEI', 'Patricia Palio de Paulo', '2792745346', 12), (2547, 'Alimentos Fit', '961923079000189', 'Ana M. Sodre ME', 'Ana Marques Sodre', '2798450798', 13), (2548, 'Lavanderia Lavou Tá Novo', '270123430000106', 'Lucinda Benedita ME', 'Lucinda Benedita', '2792359483', 14), (2549, 'Acessórios do Bem', '961923009000290', 'VR utilidades e moda', 'Thiago Benevindo Soares', '21981332256', 15), (2550, 'MF Estamparia', '273423471000199', 'Estampas e tecnologia S.A.', 'Mirela Freitas', '2733990020', 16), (2551, 'Imafar Vila velha', '03365852000222', 'Cromo - Comercio E Manipulacao De Produtos Farmaceuticos Ltda', 'Rodrigo Possato', '27981337111', 17), (2552, 'Itown', '441234881000100', 'Itown Saraiva e Siciliano S.a.', 'Eduardo Soares', '2799722100', 18);

>> insert into ENTREGADU (cod_entregador, nome, meio_transporte, telefone, data_nascimento, cpf) values (2245, 'Pedro Henrique Santos', 'minivan', '2796359890', '1998-12-21', '12490832700'), (2246, 'Jeorge Paulo Duarte', 'moto elétrica', '27902833948', '1988-12-3', '14503923703'), (2247, 'Santos De Sá', 'carro', '27944325435', '1999-2-23', '14175924712'), (2248, 'Sidoca De Souza', 'Bicicleta', '27999203421', '1992-11-24', '11194488788'), (2249, 'Renato Ferreira', 'Bicicleta', '27902930092', '1990-1-10', '15806403700'), (2250, 'Diana Cardoso', 'patinete', '27911230908', '1990-6-9', '10640712755'), (2251, 'Miria Silva', 'moto', '27934511154', '1993-1-2', '11200711703'),
(2252, 'Carla Souza Alvarenga', 'Bicicleta', '2799778421', '1989-3-14', '10500930733'); 

>> insert into  CLIENTE (cod_cliente, nome, telefone) values (2245, 'Pedro Joao de Lukas', '27937289654'), (2246, 'Marcia Santiago', '27917352009'), (2247, 'Gabrielle Santos', '27921328809'), (2248, 'Luiz Marcos Souza', '27999288754'), (2249, 'Ramom Wesley', '27911991560'), (2250, 'Deivid Jorgete Lanzini', '2799990293'), (2251, 'Fernanda Gomes', '2799893345'), (2252, 'Carla Santos de Sá', '27977899911'), (2253, 'Cecilia Antunes', '27917352010'), (2254, 'Rita Azevedo', '27921328810'), (2255, 'Eduardo Magnago', '27999288755');

>> insert into  ENCOMENDA (cod_encomenda, nomeprod, descricao, quantidade, data_entrega, hora_retirada,  >>id_lojista, cod_cliente, id_endereco) values (2023, 'comida', 'kit de 7 saladas, 3 sobremesas e 5 sucos desintoxicantes', '1', '2021-3-24', '12:00', 2547, 2245, 19), (2234, 'comida', 'pasteizinhos de sabores variados congelados, peso 3kg', '300', '2021-3-24', '13:00', 2544, 2246, 20), (2445, 'comida', 'kibe de carne congelado para festa', '100', '2021-3-24', '13:00', 2544, 2247, 21), (2656, 'roupa', 'vestido feminio', '1', '2021-3-24', '12:00', 2545, 2248, 22), (2867, 'roupa', 'conjunto de blusa e calça feminino', '1', '2021-3-24', '11:00', 2545, 2249, 23), (3078, 'roupa de cama', 'edredon lavado e passado', '1', '2021-3-24', '10:00', 2548, 2250, 24), (3289, 'sapato', 'bota para construção civil e sapato de salto', '2', '2021-3-25', '09:00', 2546, 2251, 25),
(3500, 'comida', 'kit de frutas congeladas para smoothie', '4', '2021-3-25', '10:00', 2547, 2252, 20), (3711, 'comida', 'kit de frutas congeladas para smoothie', '2', '2021-3-25', '09:00', 2547, 2250, 21), (4133, 'utensilios casa', 'mesa de canto', '1', '2021-3-25', '12:00', 2549, 2254, 22), (4344, 'roupa', 'jogo de camisas decorativas', '14', '2021-3-25', '11:00', 2550, 2253, 26), (4555, 'remédio', 'remedios manipulados caixa pequena', '6', '2021-3-26', '10:00', 2551, 2254, 27), (4766, 'eletroeletrônico', 'lampada led mesa multicolor', '1', '2021-3-26', '09:00', 2552, 2255, 28); 

>> insert into  escolhe (id_area, cod_entregador) values (1002, 2245), (1003, 2246), (1001, 2247), (1004, 2248), (1005, 2249), (1006, 2250), (1004, 2251), (1001, 2252); 

>> insert into entrega (cod_entregador, cod_encomenda) values (2248, 2023), (2248, 2234), (2249, 2445), (2246, 2656), (2247, 2867), (2247, 3078), (2245, 3289), (2251, 3500), (2249, 3711), (2246, 4133), (2245, 4344), (2245, 4555), (2245, 4766); 


### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
          
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>

>>select * from Area_geografica;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/select*from/select%2001.JPG" >

>>select * from ENDERECO;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/select*from/select%2002.JPG" >

>>select * from LOJISTA;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/select*from/select%2003.JPG" >

>>select * from ENTREGADU;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/select*from/select%2004.JPG" >

>>select * from CLIENTE;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/select*from/select%2005.JPG" >

>>select * from ENCOMENDA;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/select*from/select%2006.JPG" >

>>select * from escolhe;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/select*from/select%2007.JPG" >

>>select * from entrega;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/select*from/select%2008.JPG" >



#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>

>>select * from ENCOMENDA where nomeprod = 'comida';
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/where/where%2001.JPG" >


>>select * from ENCOMENDA where data_entrega = '2021-3-25';
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/where/where%2002.JPG" >

>>select * from ENDERECO where id_area = 1003 ;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/where/where%2003.JPG" >

>>select * from escolhe where id_area = 1003 ;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/where/where%2004.JPG" >

>>select * from entrega where cod_entregador = 2246 ;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/where/where%2005.JPG" >


#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOSsq
    a) Consultas que envolvam os operadores lógicos AND, OR e Not
    
    
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


