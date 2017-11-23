# EEL840-KDD-CUP-99

## Contexto do tema abordado

Nossa proposta é analisar o dataset do KDD Cup de 1999 contendo dados de diversos 
tipos de ataques simulados pela DARPA na rede da Força Aérea Americana em 1998.

Esse dataset contém 4.898.431 registros *(dos quais inicialmente usaremos 10% por limitações computacionais)* e 31 features, sendo elas:


** Variáveis básicas relacionadas ao TCP **

---
| Nome| Descrição | Tipo  |
|---|---|---|
|duration|número de segundos da conexão|contínua|
|protocol_type|tipo de protoclo usado *(ex: tcp,udp,etc)*|discreta|
|service|tipo de servico de rede no destino *(ex: http,telnet)*|discreta|
|src_bytes|número de bytes transferidos da origem até o destino|contínua|
|dst_byte|números de dados transferidos do destino até a origem|contínua|
|flag|status de erro da conexão|discreta|
|land|1 se a conexão é para o mesmo host/porta|discreta|
|wrong_fragments|número de fragmentos errados|contínua|
|urgent|número de pacotes urgentes|contínua|


**Outras variáveis**

| Nome| Descrição  | Tipo  |
|---|---|---|
|hot|número de *hot indicators*| contínua|
|num_failed_logins|número de tentativas de login que falharam|contínua|
|logged_in|1 se está logado com sucesso|discreta|
|num_compromised|número de condições comprometidas|contínua|
|root_shell|1 se o *root shell* foi obtido|discreta|
|su_attempt| 1 se o commando *su root* foi tentado|discreta|
|num_root|número de acessos do tipo *root*|contínua|
|num_file_creations|número de operações de criação de arquivos|contínua|
|num_shells|númerode shells iniciados|contínua|
|num_access_files|número de operações nos arquivos de controle de acesso|contínua|
|num_outbound_cmds|númer de comandos de saída em uma sessão FTP|contínua|
|is_hot_login|1 se o login pertece a list *hot*|discreta|
|is_guest_login|1 se o login é feito por um convidado|discreta|
|count|número de conexões para o mesmo host que a conexão atual nos últimos 2 segundos |contínua|
|serror_rate|% das conexões que possuem SYN error|contínua|
|rerror_rate|% das conexões que possuem REJ error|contínua|
|same_srv_rate|% das conexões para o mesmo serviço|contínua|
|diff_srv_rate|% das conexões para diferentes serviços|contínua|
|srv_cont|número de conexões para o mesmo serviço que o atual nos últimos 2 segundos|contínua|
|srv_serror_rate|% das conexões que possuem SYN error (em conexão de mesmo serviço)|contínua|
|srv_rerror_rate|% das conexões que possuem REJ error (em conexão de mesmo serviço)|contínua|
|srv_diff_host_rate |% das conexões para hosts diferentes|contínua|



## Problema específico envolvendo o tema abordado
Conseguir classificar se a detecção um determinado padrão de features caracteriza ou não um ataque. Ainda, descobrir quais são as features que melhor caracterizam cada tipo de ataque.

##Proposta de Implementação

Para a análise pretendemos testar diversas técnicas de aprendizado de máquina, desde modelos de classificação até modelos de clusterização. Alguns dos exemplos de modelos que pretendemos testar são regressão logística, k-means, classificadores bayesianos, redes neurais e SVMs. Além disso, pretendemos criar visualizações eficientes e que permitam extrair informações interessantes​ ​dos​ ​dados,​ ​tais​ ​como​ ​histogramas,​ ​boxplots,​ ​matrizes​ ​de​ ​covariância​ ​e​ ​afins.

## Resultados esperados
Esperamos ser capazes de classificar com um grau maior que 70% de certeza se um conjunto de features caracteriza um ataque ou não. Além disso, pretendemos descobrir as 3 features que melhor caracterizam cada tipo de ataque (DoS,  Probins, R2L & U2R).

## Referências

Referências Bibliográficas

[1] Dataset: http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html

[2] GIRMA, Anteneh; GARUBA, Mosses; GOEL, Rajini. Advanced Machine Language Approach to Detect DDoS Attack Using DBSCAN Clustering Technology with Entropy. In: Information Technology-New Generations. Springer, Cham, 2018. p. 125-131.

[3] LI, Qingru et al. An Intrusion Detection System Based on Polynomial Feature Correlation Analysis. In: Trustcom/BigDataSE/ICESS, 2017 IEEE. IEEE, 2017. p. 978-983.

[4]  TAVALLAEE, Mahbod et al. A detailed analysis of the KDD CUP 99 data set. In: Computational Intelligence for Security and Defense Applications, 2009. CISDA 2009. IEEE Symposium on. IEEE, 2009. p. 1-6.

[5] Lincoln Laboratory - https://www.ll.mit.edu/ideval/docs/attackDB.html

[6] http://shodhganga.inflibnet.ac.in/bitstream/10603/9850/8/08_chapter%203.pdf
