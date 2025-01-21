# Documento de Visão

## Histórico de Revisões

| Data                |  Versão             |          Descrição  |  Autores            |
| -----------------   | -----------------   | -----------------   | -----------------   |
| 25/12/2024 | 1.0 | Primeira versão | Ana Célia Baía Araújo | 

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

## 10. Regras de negócio

| Código | Nome | Descrição |
| ------------- | ------------- | ------------- |
| RN01 | Limitação de cadastro de ações | Um Colaborador não pode criar mais de três ações |
| RN02 | Acesso a ações | Em ações "fechadas" (não-públicas), um voluntário precisa ter seu acesso permitido pelo responsável da ação para ver informações sensíveis sobre ela. |
| RN03 | Requisito para avaliar ação | Um voluntário só pode avaliar uma ação em que participou. |
| RN04 | Impedimento de spamming por denúncia | Um usuário não pode fazer mais de 3 denúncias ao mesmo usuário/evento na mesma semana.
| RN05 | Critérios de denúncia do ação | Inverdade da proposta da ação,  entre outros. | 
| RN06 | Critérios de denúncia do usuário | Discurso de ódio, comportamento suspeito, entre outros. | 

## 11. Casos de uso por ordem de prioridade

1. [CDU-001 - Autorizar voluntário na ação](../cdu/cdu-001/detalhamento-001.md)
2. [CDU-002 - Voluntariar em uma ação](../cdu/cdu-002/detalhamento-002.md)
3. [CDU-003 - Visualizar Ação](../cdu/cdu-003/detalhamento-003.md)
4. [CDU-004 - Buscar ações](../cdu/cdu-004/detalhamento-004.md)
5. CDU-005 - Criar ação
6. CDU-006 - Convidar responsável para uma ação
7. CDU-007 - Remover responsável de uma ação
8. CDU-008 - Desvoluntariar de uma ação
9. CDU-009 - Remover voluntário de uma ação
10. CDU-010 - Avaliar voluntário
11. CDU-011 - Avaliar ação
12. CDU-012 - Gerenciar ação
13. CDU-013 - Gerenciar usuário
14. CDU-014 - Denunciar ação
15. CDU-015 - Denunciar usuário
16. CDU-016 - Criar conta
17. CDU-017 - notificar usuário

## 12. Glossário

|  Termo  |  Explicação  |
| ------- | ------------ |
| Ação | evento organizado por pessoas com objetivo de promover atividades que beneficiem a sociedade de forma gratuita |
| Administrador | Usuários com permissões para alterar ações, perfis dos usuários e fazer a moderação da plataforna |
| Avaliação | É a forma que um voluntário pode dar feedback de uma ação para o responsável e para os visitantes |
| Colaborador | Usuários cadastrados com login, que não são administradores |
| Responsável | Usuários que criam ações ou são adicionados como responsáveis por outro Responsável de uma ação |
| Visitante | Usuários não cadastrados na plataforma e que a utilizam |
| Voluntário | Usuários que tem sua solicitação de participação em ação aceita por um Responsável da ação |

## 13. Mensagens padrão

|   Contexto de uso  | Mensagem | 
| ------------------ | ---------------------------- | 
| Criar ação | Ação criada com sucesso!| 
| Pesquisa sem resultados| Não foi encontrado nenhum resultado para esta pesquisa.|
| Solicitação para participar de ação como voluntário(a)| Que ótimo, recebemos sua solicitação para ser voluntário(a) nesta ação, será de grande ajuda. Em breve você receberá a resposta!| 
|Resposta de aceite à solicitação para participar de ação como voluntário(a)| Sua solicitação para participar de ação como voluntário(a) foi aceita! Estamos muito felizes com sua ajuda!|
|Resposta de recusa à solicitação para participar de ação como voluntário(a)| Infelizmente sua solicitação para participar de ação como voluntário(a) foi recusada! Veja em "detalhes" os motivos para a recusa. Mas não fique triste, temos várias outras ações feitas para você, não desista de continuar ajudando! botão "Detalhes"|
|Convite para tornar voluntário um responsável na ação| Você foi convidado(a) para se tornar uma das pessoas responsáveis por esta ação. Você aceita? botões "Sim"/"Não"|
|Ausência de solicitações pendentes para voluntários(as) em ação| Não há novas solicitações para participação na ação.|
|Remoção de responsável| Você foi removido(a) da função de responsável nesta ação.|
|Remoção de voluntário| Você foi removido(a) desta ação enquanto voluntário(a).|
|Solicitação para desistir de ação como responsável| Recebemos sua solicitação para deixar de ser responsável nesta ação, que pena mas imprevistos acontecem! Aguardamos você na organização de outras ações em outras oportunidades... Continue ajudando, todos por um bem comum!|
