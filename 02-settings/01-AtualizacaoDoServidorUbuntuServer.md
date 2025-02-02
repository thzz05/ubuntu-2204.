#Autor: Robson Vaamonde<br>
#Procedimentos em TI: http://procedimentosemti.com.br<br>
#Bora para Prática: http://boraparapratica.com.br<br>
#Robson Vaamonde: http://vaamonde.com.br<br>
#Facebook Procedimentos em TI: https://www.facebook.com/ProcedimentosEmTi<br>
#Facebook Bora para Prática: https://www.facebook.com/BoraParaPratica<br>
#Instagram Procedimentos em TI: https://www.instagram.com/procedimentoem<br>
#YouTUBE Bora Para Prática: https://www.youtube.com/boraparapratica<br>
#Data de criação: 18/04/2023<br>
#Data de atualização: 31/10/2023<br>
#Versão: 0.01<br>

Release Notes Ubuntu Server 22.04.x: https://discourse.ubuntu.com/t/jammy-jellyfish-release-notes/24668<br>
Ubuntu Advantage for Infrastructure: https://ubuntu.com/advantage<br>
Ciclo de Lançamento do Ubuntu Server: https://ubuntu.com/about/release-cycle<br>
Releases All Ubuntu Server: https://wiki.ubuntu.com/Releases

Apt-Get ou Apt A ferramenta de pacote avançada, é uma interface de usuário de software<br>
livre que funciona com bibliotecas centrais para lidar com a instalação e remoção de<br>
software no Debian e em distribuições Linux baseadas nele.

#01_ Atualizando as Listas sources.list do Apt ou Apt-Get no Ubuntu Server<br>

	#Update é utilizado para baixar informações de pacotes de todas as fontes configuradas.
	sudo apt update

#02_ Verificando todos os pacotes a serem utilizados no Ubuntu Server<br>

	#List é utilizado para listar todos os software que serão atualizados no sistema.
	sudo apt list --upgradable

#03_ Atualizando todos os software no Ubuntu Server<br>

	#Upgrade é utilizado para instalar atualizações disponíveis de todos os pacotes atualmente 
	#instalados no sistema a partir das fontes configuradas via sources.list
	sudo apt upgrade

#04_ Forçando uma atualização completa de todos os software e dependências no Ubuntu Server<br>

	#Dist-Upgrade além de executar a função de atualização, também lida de forma inteligente 
	#com as novas dependências das novas versões de pacotes
	sudo apt dist-upgrade

#05 _ Forçando uma atualização e remoção de software desnecessários no Ubuntu Server<br>

	#Full-Upgrade executa a função de atualização, mas removerá os pacotes atualmente 
	#instalados se isso for necessário para atualizar o sistema como um todo
	sudo apt full-upgrade

#06_ Removendo pacotes desnecessários no Ubuntu Server<br>

	#Autoremove é utilizado para remover pacotes que foram instalados automaticamente para 
	#satisfazer dependências de outros pacotes e agora não são mais necessários, pois as 
	#dependências foram alteradas ou os pacotes que precisavam deles foram removidos nesse 
	#meio tempo.
	sudo apt autoremove

#07_ Fazendo a limpeza dos repositórios locais e pacotes desnecessários no Ubuntu Server<br>

	#Autoclean como Clean, o autoclean limpa o repositório local de arquivos de pacotes 
	#recuperados. A diferença é que ele remove apenas arquivos de pacotes que não podem 
	#mais ser baixados e são inúteis.
	sudo apt autoclean

#08_ Limpando o cache local do sources.list no Ubuntu Server<br> 

	#Clean limpa o repositório local de arquivos de pacotes recuperados
	sudo apt clean
	sudo reboot