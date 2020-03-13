# Checklist requisicao

* Verificar se há tarefas para o seu grupo
* Assumir a tarefa.
* Fazer update inicial do trunk da solução ser alterada.
* Criar um branch para o SD ou BG específico.
* Solicitar uma cópia temporária do banco de *prod* para *dev* (com num do chamado), pedindo no chamado permissões necessárias.
* Alterar os arquivos.
* Alterar o banco.
* Fazer backups diários do seu branch.
* Atualizar a versão das montagens.
## Para homologação:
* Fazer merge periódico do trunk no seu branch.
* Solicitar uma cópia do banco de *prod* para *hom*.
* Executar o script de transformação do banco.
* Apagar pasta de scripts
* Exportar o banco:	
	* Arquivo único por objeto
	* No botão _Avançado_
		* Gerar script de USE DATABASE: __"False"__.
		* Incluir cabeçalhos descritivos: __"False"__.
		* Gatilhos de script: __"True"__.
	* Gerar para pasta de scripts (E:\SVN\ **\<NomeDoProjeto\>** \branches\ **<num_req_ou_inc>**\BD\SCRIPTS).
	* Texto ANSI.

* Publicar em homologação.
	* Executar publicação via Jenkins.
	* Executar script de transformação da base.
* Colocar informações adicionar no chamado (SD).
* Informar via chamado que a tarefa está pronta para homologar.
* Homologar com o cliente.

## Publicar em produção
* Substituir o trunk com o seu branch.
* Fazer o commit do novo trunk.
* Montar nova tag.
* Negociar uma janela de horário para publicação com o cliente.
* Avisar aos interessados de que será feita uma nova implantação.
* Criar chamado para publicar scripts de transformação;
* Executar publicação da tag no jenkins.
* Apagar seu branch local.
