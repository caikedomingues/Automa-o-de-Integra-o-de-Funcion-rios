                                                    # Automação de Integração de Funcionários

-> Sistema de Automação que irá realizar tarefas repetitivas da criação de contratos e envios de e-mails para funcionários 
que irão ingressar em uma empresa. Basicamente o sistema irá acessar planilhas presentes em uma pasta no computador
da empresa com o objetivo de usar os dados coletados para construir o contrato do funcionário e envia-lo via email.
                                                       
                                                       
                                                            Funcionalidades do Sistema

-> Antes de realizar qualquer etapa o sistema deverá criar as pastas que serão utilizadas no 
projeto.

-> O sistema devera acessar as pastas que contém as planilhas de informações.

-> Antes de realizar qualquer ação, o sistema devera verificar a extensão do arquivo para garantir que são
planilhas excel.

-> O sistema deverá coletar os dados de pessoas que irão ingressar na empresa através das planilhas.

-> O sistema devera validar os dados para saber se eles estão no formato correto de processamento.

-> O sistema deverá transferir as planilhas ja processadas para uma outra pasta.

-> O sistema deverá criar um log de erros em txt que indica o cpf e o arquivo que os dados do candidato
se encontram.

-> O sistema devera criar contratos com base no modelo de contrato definido pelo RH.

-> Por motivos de segurança contra possiveis alterações no corpo do contrato, o sistema devera
converter os contratos de docx para PDF, que torna a apresentação mais formal e permite que
o candidato acesse o contrato também pelo celular.

                                                            Itens dos Arquivos (planilhas e contratos)
-> [NOME_FUNCIONÁRIO]

-> [CPF_FUNCIONARIO]

-> [ENDERECO_FUNCIONARIO]

-> [CARGO_FUNCIONARIO]

-> [SALARIO_FUNCIONARIO]

-> [CIDADE-UF]

-> [DATA_EMISSAO].

-> [DATA_INICIO]

-> EMAIL_FUNCIONARIO

                                                            Estrutura de Pastas do Projeto

-> modelo: Pasta que irá conter o modelo de contrato que será utilizado como base para criação dos contratos

-> Planilhas: Pasta que ira conter as planilhas que serão acessadas.

-> Processados: Pasta que irá conter as planilhas já processadas.

-> Contratos: Pasta que irá conter os contratos (PDFs) criados pelo sistema.

-> Erros: Ira conter os logs com os processos que não funcionaram
                                                            Ferramentas Utilizadas

-> Python 3.12: Linguagem de programação que criará o sistema

-> Docx: Biblioteca para manipulação de documentos Word

-> pandas: Biblioteca de análise de dados que irá acessar as planilhas Excel

-> os: Biblioteca que irá criar e acessar as pastas no computador

-> smtplib: Biblioteca que irá enviar os e-mails

-> datetime: Biblioteca que irá lidar com datas e pegar as datas de emissão 
dos contratos.
