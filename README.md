# Informações:
&mdash; Nome: UserAgent;<br />
&mdash; Versão: 1.2;<br />
&mdash; Status Do Uso: Estável;<br />
&mdash; Dev.: V-Team In 2019.<br />

# Como ativar?
Vocè pode esta ativando a toda aplicação no arquivo ***autoload.php***, que se encontrar na pasta ***seucodeigniter/application/config/autoload.php*** <br />
Procurar por ***$autoload["libraries"]***, e acrescente ***'UserAgent'*** no mesmo, como no print abaixo: <br />
    EXEMPLOS:<br /> 
        - Unico:<br />
        <img style="border:2px solid red;" src="https://i.imgur.com/rqr5wwn.png" /><br />
        - Mais de um:<br />
        <img style="border:2px solid red;" src="https://i.imgur.com/vur7lQD.png" /><br />
ou acrescente no seu codigo PHP: ***$this->load->libraries('UserAgent');*** <br />
(Obs.: so está ativando para a função atual ou melhor dizendo, ativo so mente para aquele arquivo do seu sistema ou controller).

# Como usar?
Ative no seu sistema (função que irá utiliza-lo):<br /> 
  <code>
    $UserAgent = new UserAgent();<br /> | 
    Obs.: caso usar outra string no lugar de "$UserAgent" a sua string vai ser a raiz da função, mas recomendo usar a padrão.
  </code><br />
  Ultilizando:<br />
    **&mdash; Verifica o sistema operacional:** $UserAgent->checkOs(),<br />
    **&mdash; Verifica o navegador:** $UserAgent->checkBrowser(),<br />
    **&mdash; Retorna os dados da máquina que está acessando:** $UserAgent->getUserMachine(),<br />
    **&mdash; Retorna o sistema operacional da máquina que está acessando:** $UserAgent->getOs(),<br />
    **&mdash; Retorna o navegador da máquina que está acessando:** $UserAgent->getBrowser(),<br />
    **&mdash; Obtem o endereço de IP da máquina que está acessando:** $UserAgent->requestIP(),<br />
    



 
  

# Change Logs:
  @Class: Retorna dados na máquina que está acessamdo o servidor.<br />
  @log v1.2 : Adicionado método para obter o IP da máquina.<br />
 
