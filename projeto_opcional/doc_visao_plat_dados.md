# Documento de Visão

## Histórico de Revisões

| Data                |  Versão             |          Descrição  |  Autores            |
| -----------------   | -----------------   | -----------------   | -----------------   |
| 21/12/2024 | 1.0 | Primeira versão | Ana Célia Baía Araújo | 

## 1. Objetivo do projeto

Criar uma plataforma para integrar dados e informações produzidas a partir das pesquisas científicas do Laboratório Interdisciplinar Sociedade, Ambiente e Territórios - LISAT/IPP/UFRN

## 2. Descrição do problema

|     |      |
| --- | --- |
| **Problema**            | não existir um espaço virtual que integre os vários bancos de dados de indicadores produzidos e/ou utilizados pelos pesquisadores do LISAT |
| **Afeta**               | interessados em produzir estudos nas temáticas afins à relação entre Sociedade, Ambiente e Territórios |  
| **Impacta**             | a divulgação científica e reprodução das metodologias e ferramentas criadas, pois as informações produzidas ficam com acesso limitado |
| **Solução**             | construir uma plataforma que permita que interessados e instituições relacionadas às temáticas utilizar os bancos de dados e outras informações produzidas pelos pesquisadores do LISAT  | 

## 3. Descrição dos usuários 

| Nome                |  Descrição          |   Responsabilidade  |
| -----------------   | -----------------   | -----------------   |
| Administrador | Os administradores serão usuários com permissões para alterar ações e perfis dos demais usuários, e todos os outros requisitos | Gerenciar ações e usuários - Moderar o conteúdo postado - Validar denúncias sobre ações e usuários - Realizar manutenções e melhorias no sistema |
| Colaborador | Os usuários cadastrados com login, que não são administradores, poderão utilizar a plataforma para disponibilizar seus achados e produções científicas | Criar postagens; Gerenciar dados que serão disponibilizados na plataforma |
| Visitante | Os usuários que podem visualizar o site mas que, por não terem realizado cadastro ainda, não podem incluir informações/dados na plataforma.   | Os usuários não cadastrados podem: - Visualizar o conteúdo da plataforma - Se cadastrar na plataforma - Compartilhar conteúdos existentes | 

## 4. Descrição do ambiente dos usuários

A plataforma terá como página inicial uma listagem de documentos (artigos científicos, legislações, documentos técnicos), arquivos (mapas, fotos, ilustrações esquemáticas, scripts, ferramentas metodológicas, entre outros) e bancos de dados disponíveis (planilhas, tabelas, entr outros), categorizados por temática, por projeto no qual estão vinculados e por pesquisadores responsáveis por produzir esse conteúdo.

## 5. Principais necessidades dos usuários

Aplicar e analisar respostas de um questionário para levantar as necessidades entre os pesquisadores do LISAT.

REVISAR
## 6. Alternativas concorrentes


## 7. Visão geral do produto

A Plataforma Dados-SAT será um produto de acesso para toda a sociedade, com recursos de usabilidade que considerem premissas de acessibilidade e interface intuitiva. A proposta é integrar e proporcionar um ambiente para interação entre pesquisadores, mas também comunidades e gestores públicos. O produto poderá dispor aos usuários um catálogo de produtos desenvolvidos a partir dos trabalhos dos pesquisadores do LISAT, que deverá ser continuamente atualizado a partir do uso da Plataforma diretamente pelos autores, visando ampliar a divulgação das produções científicas no âmbito do Laboratório.

## 8. Requisitos funcionais

| Código              |  Nome               |          Descrição  |  Prioridade         |
| -----------------   | -----------------   | -----------------   | -----------------   |
| F01  |  Login  |  O usuário tem acesso ao sistema.  | -  |
| F02  | Cadastro de Projetos | O Colaborador cadastra uma ação de trabalho voluntário  |  - |
| F03  | Cadastro de Pesquisadores | Visitante pode se cadastrar na plataforma | - |
| F04  | Gerenciamento de conteúdo | Administrador gerencia arquivos disponíveis (atualizar e remover) | - | 
| F05  | Gerenciamento de usuários | Administrador gerencia usuários da plataforma (atualizar e remover) | - |
| F06  | Busca de produtos | usuários pesquisam produtos disponíveis | Alta | 
| F07  | Visualização de Produtos | usuários podem visualizar produtos disponíveis | Alta | 
| F08  | Cadastro do usuário como pesquisador em uma pesquisa |  Responsável do produto inclui usuário para gerenciar o produto | Alta |
| F09  | Logout | usuário sai do sistema | - |




REVISAR
## 9. Requisitos não-funcionais

| Código              |  Nome               |          Descrição  |  Categoria          |  Classificação      |
| -----------------   | -----------------   | -----------------   | -----------------   | -----------------   |
| NF01 | Segurança das informações pessoais | Os dados pessoais, endereços e outras informações dos bancos de dados da plataforma deverão estar asseguradas segundo a Lei Geral de Proteção de Dados Pessoais (LGPD). | Segurança | Obrigatório |
| NF02 | Interface acessível | Espera-se que a interface e o design sejam construídos a partir de fontes, tamanhos, imagens, ícones, esquemas de cores  e outras ferramentas que possibilitem inclusão de pessoas com problemas de visão (ferramenta de lupa, alto contraste, leitura em voz alta, etc), prezando por uma comunicação clara com os usuários | Usabilidade | Desejável |
| NF03 | Usabilidade da plataforma | Espera-se que o uso da plataforma seja intuitivo para que vários tipos de usuários (iniciais, intermediários, avançados, admin) possam navegar pelo sistema sem grandes dificuldades | Usabilidade | Desejável |
| NF04 | Confiabilidade e credibilidade | Serão estabelecidos protocolos para que os usuários tanto possam denunciar ações e/ou usuários suspeitos, como será possível um sistema de avaliação entre voluntários na plataforma sobre confiança e credibilidade das ações | Segurança | Obrigatório |
| NF05 | API externa | Utilizar API externa no sistema | Arquitetura |  Obrigatória |
| NF06 | Arquitetura Distribuída | Separar o front-end e back-end | Arquitetura | Obrigatória |

