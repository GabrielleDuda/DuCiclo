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

A plataforma DuCiclo têm a ideia de interligar motoboys, lojistas e clientes, com o objetivo de entregar com segurança qualquer coisa que possa ser carregada de maneira segura. A missão da plataforma é resolver o problema de lojistas que agora atendem delivery mas não possuem serviços próprios de entrega de mercadoria, além de gerar empregos para entregadores que não possuam carro ou moto para realizar a entrega.  Primeiramente ocorre um cadastro no aplicativo onde lojista se cadastra com CNPJ ou CPF, nome do estabelecimento ("nome fantasia"), Razão social, nome do responsável, telefone, endereço da loja. Os entregadores podem ser motoboys, ciclistas, ou usuários de qualquer forma de locomoção, desde de que façam acesso a plataforma cadastrando previamente nome, cpf, data de nascimento (para que não sejam catalogados menores de idade), meio de transporte, escolhe a área geográfica de atuação,  telefone para contato. A área geográfica vai ajudar a delimitar a atuação do entregador e assim possibilitar maior segurança no prazo para entrega das encomendas, previamente existentes na plataforma essa tem opções de grupos de bairros para atendimento. O cliente tambem pode se cadastrar com nome e telefone, sua função é acompanhar a entrega. O lojista cadastra a encomenda (nome do produto, descrição, valor, quantidade, data da entrega, hora da retirada da entrega) e estas são agrupadas por bairros proximos. O aplicativo apresenta ao entregador, de acordo com sua área, as entregas disponiveis para o dia seguinte, para que o sistema de agrupamento de áreas próximas funcione é importante salienar que as entregas tem prazo de 24horas para ocorrer. Em outras palavras, o lojista cadastra mas não serão retiradas da loja no dia de cadastro da entrega. Quando o entregaDu aceita uma encomenda  é criado o pedido, que interliga o cliente cadastrado previamente (importante o logista orientar ao cliente essa necessidade), ao entregaDu e a encomenda cadastrada pelo lojista. Entrega feita então se avalia todos os critérios por todos os envolvidos e assim a plataforma ganha em melhoria de atuação.

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
	id_lojista integer PRIMARY KEY, nomefantasia varchar(100), CNPJ varchar(15), razaosocial varchar(100), nome_resp varchar(100), telefone char(11), id_endereco integer, FOREIGN KEY (id_endereco) REFERENCES ENDERECO (id_endereco) ON DELETE RESTRICT );

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

>> insert into  ENCOMENDA (cod_encomenda, nomeprod, descricao, quantidade, data_entrega, hora_retirada, id_lojista, cod_cliente, id_endereco) values (2023, 'comida', 'kit de 7 saladas, 3 sobremesas e 5 sucos desintoxicantes', '1', '2021-3-24', '12:00', 2547, 2245, 19), (2234, 'comida', 'pasteizinhos de sabores variados congelados, peso 3kg', '300', '2021-3-24', '13:00', 2544, 2246, 20), (2445, 'comida', 'kibe de carne congelado para festa', '100', '2021-3-24', '13:00', 2544, 2247, 21), (2656, 'roupa', 'vestido feminio', '1', '2021-3-24', '12:00', 2545, 2248, 22), (2867, 'roupa', 'conjunto de blusa e calça feminino', '1', '2021-3-24', '11:00', 2545, 2249, 23), (3078, 'roupa de cama', 'edredon lavado e passado', '1', '2021-3-24', '10:00', 2548, 2250, 24), (3289, 'sapato', 'bota para construção civil e sapato de salto', '2', '2021-3-25', '09:00', 2546, 2251, 25),
(3500, 'comida', 'kit de frutas congeladas para smoothie', '4', '2021-3-25', '10:00', 2547, 2252, 20), (3711, 'comida', 'kit de frutas congeladas para smoothie', '2', '2021-3-25', '09:00', 2547, 2250, 21), (4133, 'utensilios casa', 'mesa de canto', '1', '2021-3-25', '12:00', 2549, 2254, 22), (4344, 'roupa', 'jogo de camisas decorativas', '14', '2021-3-25', '11:00', 2550, 2253, 26), (4555, 'remédio', 'remedios manipulados caixa pequena', '6', '2021-3-26', '10:00', 2551, 2254, 27), (4766, 'eletroeletrônico', 'lampada led mesa multicolor', '1', '2021-3-26', '09:00', 2552, 2255, 28); 

>> insert into  escolhe (id_area, cod_entregador) values (1002, 2245), (1003, 2246), (1001, 2247), (1004, 2248), (1005, 2249), (1006, 2250), (1004, 2251), (1001, 2252); 

>> insert into entrega (cod_entregador, cod_encomenda) values (2248, 2023), (2248, 2234), (2249, 2445), (2246, 2656), (2247, 2867), (2247, 3078), (2245, 3289), (2251, 3500), (2249, 3711), (2246, 4133), (2245, 4344), (2245, 4555), (2245, 4766); 


### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
          
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>

COLAB : https://colab.research.google.com/drive/18_EpkzlgGRnyzZhDIQQunSn9MoO7I-Qf?usp=sharing

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

>>select *from ENDERECO where (id_area = 1003 or id_area = 1004 );
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/And%2C%20or%2C%20not/aritmetica%20001.JPG" >

>>select cod_encomenda from ENCOMENDA where (quantidade >10 and quatidade<100);
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/And%2C%20or%2C%20not/aritmetica%20002.JPG" >

>>select *from ENCOMENDA where (id_lojista = 2544 or id_lojista = 2547);
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/And%2C%20or%2C%20not/aritmetica%20003.JPG" >

>>select nome from ENTREGADU where meio_transporte not in ('Bicicleta');
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/And%2C%20or%2C%20not/aritmetica%20004.JPG" >

>>select *from area_geografica where cidade not in ('SERRA');
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/And%2C%20or%2C%20not/aritmetica%20005.JPG" >

    
    b) Criar consultas com operadores aritméticos 
 
 No caso da proposta apresentada no trabalho, tais cálculos não se fazem tão utéis apenas para finalidade de médias. Outros operadores como count podem ajudar a estabelecer relatórios mais reais. Porém, como critério de nota, duas sugestões de contas foram propostas.
 
 
>>média de entregas por entregadores:
    select (qtd_encomendas / qtd_entregadores ) as media 
	from ( select count(cod_entregador) as qtd_entregadores,
	(select count(cod_encomenda) from ENCOMENDA) as qtd_encomendas from ENTREGADU ) as quantidades;
 <img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/operadores%20aritmeticos/aritmetica%20006.JPG" >


>>porcentagem de entregas por lojista (o elephantsql arredonda os resultados): 
    select ((qtd_loja / qtd_entregas )*100 ) as porcentagem 
	from ( select count(id_lojista='2547') as qtd_loja,
	(select count(cod_encomenda) from ENCOMENDA) as qtd_entregas from ENCOMENDA) as quantidades;
 <img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/operadores%20aritmeticos/aritmetica%20007.JPG" >


    c) Consultas com operação de renomear nomes de campos ou tabelas

>> select loragradouro AS Logradouro FROM ENDERECO;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/rename/imagem001.JPG" >

>> ALTER TABLE ENTREGADU RENAME TO ENTREGADOR ;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/rename/imagem002.JPG" >

>> select cod_entregador AS id_entregadu FROM ENTREGADU;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/rename/imagem003.JPG" >

>> select nomeprod AS tipo_produto FROM ENCOMENDA;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/rename/imagem004.JPG" >



#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS  <br>
    a) Criar consultas que envolvam like ou ilike
 
Buscando nome de bairro:
>> select *from endereco where bairro like '%atima'; 
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/like%20or%20ilike/Capturar01.JPG" >

Quais itens vem em maior quantidade:
>> select *from encomenda where descricao like 'kit%';
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/like%20or%20ilike/Capturar02.JPG" >

Buscando o nome de um cliente:
>> select *from cliente where nome like 'C%';
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/like%20or%20ilike/Capturar03.JPG" >

Buscando nome comercial de loja com letra M:
>> select *from lojista where nomefantasia ilike 'm%';
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/like%20or%20ilike/Capturar04.JPG" >

Buscando ruas cadastradas nos endereços:
>> select *from endereco where logradouro ilike 'rua%'
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/like%20or%20ilike/Capturar05.JPG" >

Buscando entregador com a letra S:
>>select *from entregador where nome ilike 'S$';
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/like%20or%20ilike/Capturar05.JPG" >


    b) Criar uma consulta para cada tipo de função data apresentada.
 
Buscando a idade dos entregadores cadastrados:
>> select nome, current_date as data_atual, data_nascimento, (age(current_date, data_nascimento)) from entregador;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/DATE/Capturar01.JPG">

Buscando os dias de entregas:
>> select DATE_PART('day', data_entrega) as dia from encomenda;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/DATE/Capturar02.JPG">

Buscando o dia cadastrado as encomendas:
>> select  data_entrega  - interval '1 day' as novo  from encomenda ;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/DATE/Capturar03.JPG">

Buscando a quantos dias as entregas foram realizadas:
>> select data_entrega ,(age(current_Date, data_entrega)) as tempo from encomenda ;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/DATE/Capturar04.JPG">



#### 9.5	INSTRUÇÕES APLICANDO ATUALIZAÇÃO E EXCLUSÃO DE DADOS <br>
    a) Criar instrução de exclusão
    /*A instrução delete foi testada mas não implementada para que não ocorrer perdas de valores no trabalho*/

>>delete from cliente where cod_cliente = 2248;

>>delete from entrega where cod_encomenda = 2234;

    b) Criar funções de atualização
    /*utilizando instrução update*/
    
>>update cliente set nome = 'João Pedro Lucas' where nome = 'Pedro Joao de Lukas';
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/update/Capturar1.JPG">

>>update entregador set meio_transporte = 'mini-van' where meio_transporte = 'minivan';
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/update/Capturar2.JPG">

>>update entregador set meio_transporte = 'moto como baú' where meio_transporte = 'moto';
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/update/Capturar3.JPG">

>>update entregador set nome = 'Sidney Soares de Souza' where nome = 'Sidoca De Souza';
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/update/Capturar4.JPG">



#### 9.6	CONSULTAS COM INNER JOIN E ORDER BY <br>

    a) junção que envolva todas as tabelas possuindo no mínimo 2 registros no resultado
	/pedidos do cliente 2248/
SELECT * from encomenda 
 join cliente on (encomenda.cod_cliente = cliente.cod_cliente)
 where encomenda.cod_cliente = 2248 order by cod_encomenda;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/inner%20join%2C%20order%20by/Capturar.JPG">


  	/descriação da entrega do entregador 2249/
select  encomenda.cod_encomenda,encomenda.descricao from entregador
join entrega on (entregador.cod_entregador = entrega.cod_entregador)
join encomenda on (entrega.cod_encomenda = encomenda.cod_encomenda)
where entregador.cod_entregador = 2249
order by entregador.cod_entregador;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/inner%20join%2C%20order%20by/Capturar02.JPG">


	/* loja que a cliente Fernanda comprou*/
select encomenda.cod_encomenda,lojista.nomefantasia, cliente.nome from cliente 
join encomenda on (cliente.cod_cliente = encomenda.cod_cliente)
join lojista on (encomenda.id_lojista = lojista.id_lojista) 
where cliente.nome ilike 'Fernanda%' ;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/inner%20join%2C%20order%20by/Capturar03.JPG">


	/* nome do cliente que comprou mesa de canto*/
select encomenda.cod_encomenda,encomenda.descricao,cliente.nome from encomenda
join cliente on (encomenda.cod_cliente = cliente.cod_cliente)
where encomenda.descricao like "%mesa de canto%";
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/inner%20join%2C%20order%20by/Capturar04.JPG">


	/*apresentar bairros e tipos de produtos*/
select encomenda.cod_encomenda,bairro,encomenda.nomeprod from encomenda
join endereco on (encomenda.id_endereco = endereco.id_endereco) 
order by encomenda.cod_encomenda;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/inner%20join%2C%20order%20by/Capturar05.JPG">
    

#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO <br>
    
    a) Criar minimo 2 envolvendo algum tipo de junção

	/*consulta pessoa e seu cpf*/
  SELECT nomefantasia, CNPJ FROM lojista GROUP BY nomefantasia, CNPJ;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/group%20by%20e%20agrupamento/Capturar.JPG">

	/*consulta cep e nome da rua*/
SELECT CEP, loragradouro FROM ENDERECO GROUP BY CEP, loragradouro;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/group%20by%20e%20agrupamento/Capturar02.JPG">

	/*conta a quantidade de encomenda por loja*/
SELECT encomenda.id_lojista, lojista.nomefantasia, count(encomenda.id_lojista) as qtd_encomendas
FROM encomenda INNER JOIN lojista ON encomenda.id_lojista = lojista.id_lojista  GROUP BY encomenda.id_lojista, lojista.nomefantasia ;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/group%20by%20e%20agrupamento/Capturar03.JPG">

	/*conta a quantidade de encomenda por cliente*/
SELECT encomenda.cod_cliente, cliente.nome, count(encomenda.cod_cliente) as qtd_pedidos FROM encomenda INNER JOIN cliente ON encomenda.cod_cliente = cliente.cod_cliente  GROUP BY encomenda.cod_cliente, cliente.nome ;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/group%20by%20e%20agrupamento/Capturar04.JPG">
  
	/*conta a quantidade de endereços por area*/
SELECT  endereco.id_area, area_geografica.nome, count(endereco.id_endereco) as qt_bairros FROM endereco INNER JOIN area_geografica ON  endereco.id_area = area_geografica.id_area  GROUP BY endereco.id_area, area_geografica.nome ;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/group%20by%20e%20agrupamento/Capturar05.JPG">
  
    
  
    
    

#### 9.8	CONSULTAS COM LEFT, RIGHT E FULL JOIN <br>

 /* cliente que comprou qual produto */
select encomenda.nomeprod as produto, cliente.nome AS comprador from encomenda 
right join cliente on (encomenda.cod_cliente=cliente.cod_cliente);
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/left%2C%20right%2C%20full/Capturar01.JPG">
  

/* loja resposanvel por cada produto*/
select encomenda.descricao as produto, lojista.nomefantasia AS Loja from encomenda 
right join lojista on (encomenda.id_lojista=lojista.id_lojista);
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/left%2C%20right%2C%20full/Capturar02.JPG">
  

/* bairro e sua area geografica*/
select  endereco.bairro, area_geografica.id_area from endereco
left join area_geografica on (endereco.id_Area=area_geografica.id_area)
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/left%2C%20right%2C%20full/Capturar03.JPG">
  

/* loja em cada bairro*/
select lojista.nomefantasia, endereco.id_endereco, lojista.nome_resp
from endereco full outer join lojista
on (lojista.id_endereco = endereco.id_endereco);
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/left%2C%20right%2C%20full/Capturar04.JPG">
  


#### 9.9	CONSULTAS COM SELF JOIN E VIEW <br>
    As consultas com self join não condizem com a tabela de dados do projeto, pois não possuem entidades auto relacionadas no caso. Por isso foi feita uma view para complementar a questão:
    
	/*View que sintetiza a tabela de encomenda*/
    create view pedido as select nomeprod as tipo, descricao as descrição, data_entrega as cadastro  from encomenda; select *from pedido"
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/select*from/view.JPG">
  
#### 9.10	SUBCONSULTAS <br>

	/*relação entregador, area geografica e o bairro*/
>>select entregador.nome, area_geografica.id_area, escolhe.id_area
	from entregador
	inner join escolhe on
	(entregador.cod_entregador=escolhe.cod_entregador)
	inner join area_geografica on
	(escolhe.id_Area=area_geografica.id_area)
	group by area_geografica.nome, entregador.nome, area_geografica.id_area,  escolhe.id_area;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/subconsulta/Capturar01.JPG">
		
	/*relação loja, área geografica e cliente*/
>>SELECT lojista.nomefantasia,cliente.nome,area_geografica.nome from encomenda 
	join cliente on (encomenda.cod_cliente = cliente.cod_cliente)
	join endereco on (encomenda.id_endereco = endereco.id_endereco)
	join lojista on (encomenda.id_lojista = lojista.id_lojista) 
	join area_geografica on (area_geografica.id_area = endereco.id_area )
		order by lojista.nomefantasia;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/subconsulta/Capturar02.JPG">


	/*relação bairro, cliente e data de encomenda*/
>> SELECT encomenda.data_entrega,cliente.nome,endereco.bairro from encomenda 
	join cliente on (encomenda.cod_cliente = cliente.cod_cliente)
 	join endereco on (encomenda.id_endereco = endereco.id_endereco) 
		order by cod_encomenda;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/subconsulta/Capturar03.JPG">


	/*relação nome fantasia, dia da encomenda e qual entregador vai entregar*/
>>Select  encomenda.data_entrega,encomenda.descricao,lojista.nomefantasia,entregador.nome from entregador
	join entrega on (entregador.cod_entregador = entrega.cod_entregador)
	join encomenda on (entrega.cod_encomenda = encomenda.cod_encomenda)
	join lojista on (encomenda.id_lojista = lojista.id_lojista) 
		order by entregador.cod_entregador;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/subconsulta/Capturar04.JPG">


	/* area, entregador*/
>>SELECT lojista.nomefantasia,cliente.nome,area_geografica.nome from encomenda 
 	join cliente on (encomenda.cod_cliente = cliente.cod_cliente)
 	join endereco on (encomenda.id_endereco = endereco.id_endereco)
 	join lojista on (encomenda.id_lojista = lojista.id_lojista) 
	join area_geografica on (area_geografica.id_area = endereco.id_area )
		order by lojista.nomefantasia;
<img src="https://github.com/GabrielleDuda/DuCiclo/blob/main/imagens/screeenshot/subconsulta/Capturar05.JPG">


### 10 RELATÓRIOS E GRÁFICOS

### a) análises e resultados provenientes do banco de dados desenvolvido (usar modelo disponível)

![Apresentação dos relatórios]
(https://colab.research.google.com/drive/1zY9l7elOsnLhMtn97cIP0SM2kzk4wQNO?usp=sharing)
    

### 11	AJUSTES DA DOCUMENTAÇÃO, CRIAÇÃO DOS SLIDES E VÍDEO PARA APRESENTAÇAO FINAL <br>

#### a) Modelo (pecha kucha)<br>
https://github.com/GabrielleDuda/DuCiclo/blob/main/arquivos/Modelo%20(pecha%20kucha)%20-%20DuCiclo.pdf

#### b) Tempo de apresentação 6:40 


<br>
<br>
<br> 


