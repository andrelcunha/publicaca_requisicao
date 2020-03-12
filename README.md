# publicaca_requisicao

* Verificar se há tarefas para o seu grupo
* Assumir a tarefa.
* Fazer update inicial do trunk da solução ser alterada.
* Criar um branch para o SD ou BG específico.
* Alterar os arquivos.
* Fazer backups diários do seu branch.
* Atualizar a versão das montagens.
**Para homologação:** 
	* Fazer merge periódico do trunk no seu branch.
	* Alterar o banco.
	* Exportar o banco.
  	* Apagar pasta de scripts
    * Arquivo único por objeto
    * Avançado
      * Gerar script de USE DATABASE: False
      * Incluir cabeçalhos descritivos: False
      * Gatilhos de script: True
		* Gerar para pasta de scripts (E:\SVN\<NomeDoProjeto>\branches\<num_req_ou_inc>\BD\SCRIPTS)
		* Texto Ansi

  * Publicar em homologação.
    *	Executar publicação via Jenkins
	  *	Executar script de transformação da base
  * Criar tag
	* Colocar informações adicionar no chamado (SD).
	* Informar via chamado que a tarefa está pronta para homologar.
* Homologar com o cliente.
* Substituir o trunk com o seu branch.
* Fazer o commit do novo trunk.
* Montar nova tag.
* Publicar em produção
	* Avisar aos interessados de que será feita uma nova implantação.
	* Criar chamado para publicar scripts de transformação;
	* Executar publicação da tag no jenkins
Apagar seu branch local.
