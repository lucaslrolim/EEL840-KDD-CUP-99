# EEL840-KDD-CUP-99


## Variáveis utilizadas

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