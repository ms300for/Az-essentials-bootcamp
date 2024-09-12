## 1.1 Gerenciamento de Projetos

Projetos de _softwares_, mesmo que mantidos por uma pessoa, necessitam de um estudo sobre manutenção e expansão. Para projetos grandes e/ou com múltiplos contribuintes, o processo de versionamento torna-se essencial para a continuidade e garantia de funcionamento.

Entre os principais problemas que implicam na necessidade de versionamento, tem-se:

* Trabalho em paralelo: vários contribuintes podem estar alterando os mesmos arquivos ao mesmo tempo. Gerenciar essas modificações demanda muito esforço e torna-se inviável em projetos extensos;
* Linha do tempo: de tempos em tempos, versões estáveis de uma aplicação são entregues ao público. Controlar quais _features_ e correções serão disponibilizadas em cada lançamento é necessário para ter-se um histórico de evolução da aplicação;
* Atualização de ambiente: manter os arquivos de um projeto sempre atualizados e funcionais torna-se desafiador com diversas mudanças de código entrando com o tempo;

Visto a dificuldade de gerenciar manualmente os arquivos de um projeto, surgem programas objetivando tal ação: **os sistemas de controles de versão**. Esses sistemas gerenciam e guardam o histórico de edições, com data, autor e quais linhas foram modificadas.
Existem basicamente dois tipos:

VCS centralizados: Exemplificados pelos _softwares_ **CVS** e _**Subversion**_, o VCSC condensam as codificações em um servidor centralizado. O processo de uso é sempre _online_, necessitando acesso constante a _internet_.  

VCS distribuídos: Exemplificados pelo GIT e Mercury: funciona de forma parecida aos sistemas centralizados, porém cada área de trabalho possui uma cópia do servidor, que pode ser atualizada conforme o necessário. O processo de envio para o servidor principal é onde ocorre a resolução de conflitos de estado.
## 1.2 GIT

Criado por [Linus Torvards](https://pt.wikipedia.org/wiki/Linus_Torvalds), o sistema de versionamento GIT é o principal sistema de versionamento do mercado. Sendo gratuito e de código aberto, é um sistema leve e de fácil uso, baseado em estruturas de ramificações e entrega de pacotes.
[Documentação do GIT](https://git-scm.com/downloads)

Estruturas do GIT:
* Repositório: representa a unidade total do projeto. É a junção de todos os arquivos (e seus históricos) presentes em um ambiente de desenvolvimento.
* _Commit_: unidade básica de alteração em um repositório. Cada conjunto de alterações feitas a partir de uma referência é condensada em um _commit_. Assim, é possível segmentar conjuntos de mudanças feitas em um código e ordena-las temporalmente, facilitando o processo de reversão, atualização e de resolução de conflitos.
* _Branch_: representa uma "linha do tempo" em determinado repositório. A possibilidade de multiplas branchs permitem a existência de múltiplas linhas do tempo de _commits_ em paralelo. O processo de união (_merge_) de _branchs_ é facilitado pela possibilidade de unificação da linha do tempo, com a união automática de commits não conflitantes. Para o caso de conflitos, é possível observar como cada uma das modificações

Existem diversos serviços de hospedagem utilizando a tecnologia GIT, como bitbucket, github etc sendo o último o mais utilizado.

