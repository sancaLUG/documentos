# Guia da installfest para voluntários

Ser voluntário em uma installfest é uma tarefa difícil e que demanda
responsabilidade — apesar disso, sua experiência também será muito
gratificante. Este guia é um compilado de ideias, informações e instruções que
coletamos ao longo do tempo para ajudar nossos voluntários. Ele é baseado nos
seguintes recursos:

* [Django Girls Coaching Manual](https://coach.djangogirls.org/)
* [Guia Installfest do livrecamp](https://github.com/LivreCamp/documentos/wiki/Guia-Installfest)
* Muitas conversas com os membros do sancaLUG

## O que preciso para ser um voluntário?

Obrigado pelo interesse em voluntariar! Em nossas installfests, há várias
coisas com as quais você pode ajudar. Dentre elas, as principais atividades
são: tirar dúvidas e orientar novos usuários; realizar demonstrações de
distribuições, programas e interfaces gráficas; ajudar com a instalação e
pós-instalação das distribuições.

Para que a sua experiência seja bem-sucedida, você precisa de algumas coisas
básicas:

* Muita paciência, uma atitude gentil e amigável, além de um sorriso no rosto
* A habilidade de responder perguntas de maneira simples e amigável, mesmo que
  as respostas não sejam super precisas do ponte de vista técnico
* Tempo livre no dia do evento

## Por que devo ser um voluntário?

Além de se sentir melhor pelo trabalho voluntário, você…

* irá conhecer pessoas novas e interessantes
* provavelmente irá aprender coisas novas
* terá a gratitude eterna da comunidade de software livre e dos novos usuários

## O básico

As installfests do sancaLUG são uma oportunidade para conhecer e expandir a
comunidade de software livre de São Carlos e região. Nosso objetivo é instalar
GNU/Linux com qualidade, para que os novos usuários saiam com confiança de que
saberão utilizar o sistema e uma boa noção do que ele é. Assim, o foco é tanto
instalar o maior número de máquinas o possível, bem como gerar a maior
quantidade de conversas e educação o possível.

### Preparação anterior

Os voluntários são responsáveis por baixar as ISOs e criar os pendrives de
instalação. Recomendamos que você tenha de dois a três pendrives com
distribuições de Linux. Leve distribuições que conhece e sabe instalar; a
experiência de instalar uma distro nova será confusa tanto para você, quanto
para o usuário. Nós recomendamos as seguintes distribuições:

* [Antergos](https://antergos.com/)
* [Elementary OS](https://elementary.io/)
* [Fedora](https://getfedora.org/)
* [Manjaro](https://manjaro.org/)
* [Ubuntu MATE](https://ubuntu-mate.org/)
* [Ubuntu GNOME](https://ubuntugnome.org/)
* [Ubuntu](https://www.ubuntu.com/)

Essa lista não é, de maneira alguma, definitiva ou exaustiva. No entanto, nossa
experiência nos mostrou que essas são as distribuições mais procuradas e para
as quais há mais tutoriais e ajuda na internet. Caso você deseje levar outra
distribuição, por favor, entre em contato pelo [nosso grupo no
Telegram](https://t.me/sancaLUG).

Para criar os pendrives, recomendamos os seguintes métodos:

* [Etcher](https://etcher.io/): um aplicativo gráfico e simples de usar
* O comando `dd`, por exemplo: `dd if="caminhodaiso.iso" of="/dev/sdX" bs=4M`

Para mais informações, como por exemplo verificar a integridade de ISOs,
recomendamos o [guia de installfests do livrecamp][guia-livrecamp].

[guia-livrecamp]: https://github.com/LivreCamp/documentos/wiki/Guia-Installfest#verificando-integridade-da-iso

### Abordagem

Quando um novo usuário chegar, abra um sorriso e comece uma conversa! Pergunte
seu nome, como ficou sabendo do evento e motivação para instalar o sistema.
Explique que o sancaLUG é um grupo de tecnologia e cultura livres e que está
promovendo o evento para ajudar e expandir a comunidade. Use o que você
aprendeu sobre o usuário para determinar qual distro será instalada. Em geral,
novos usuários buscam Ubuntu. Use seu julgamento antes de recomendar uma
distribuição menos amigável para novatos, como o Gentoo, por exemplo ;)

O pedido mais comum é que a instalação seja feita ao lado do Windows, o famoso
_dual boot_. Mudar para um novo sistema é uma perspectiva assustadora, para
muitas pessoas, portanto tenha tato ao sugerir a maneira como a instalação deve
ser feita. Explique o processo de maneira simples e, antes de mais nada,
pergunte se há um backup da máquina. Peça, também, que a pessoa assine nosso
[termo de responsabilidade][termo-responsabilidade], que estará impresso e
disponível no dia do evento. Essas etapas são importantes para assegurar a
satisfação dos novos usuários e dos voluntários.

[termo-responsabilidade]: https://github.com/sancaLUG/documentos/raw/master/termo-responsabilidade.pdf

Peça permissão para usar o computador do novo usuário e agora é só instalar o
sistema! Durante todo o processo, explique os passos envolvidos na instalação
de um sistema; o objetivo é ensinar, para que os novos usuários sejam um dia
também voluntários.

Não hesite em pedir ajuda para a organização e outros voluntários, caso você
encontre algum problema. Veja também nossa [seção de dicas e resolução de
problemas comuns (em construção)](#dicas-e-problemas-comuns).

### Pós-instalação

Seu trabalho não termina com a instalação. Agora, você deve:

* Verificar o funcionamento do gerenciador de boot e se todos os sistemas estão
  inicializando corretamente
* Verificar o funcionamento dos recursos básicos, como wifi, suspensão e áudio
* Ensinar a interface básica do sistema, se já não tiver feito isso
* Mostrar como instalar novos pacotes, por meio do Software Center, por exemplo

Deixe o usuário à vontade para tirar dúvidas. Antes que ele se vá, entregue um
[formulário de feedback][formulario-feedback], que estará impresso e disponível
no dia do evento.

[formulario-feedback]: https://github.com/sancaLUG/feedback-forms/raw/master/feedback.pdf

Parabéns! Você instalou seu primeiro sistema. Agora, é só voltar para o começo
desse guia e repetir.

## Dicas e problemas comuns

Para realizar o dual boot com sucesso em computadores com os SOs Windows 8, 8.1
ou 10, é preciso desativar o Fast Boot e o Secure Boot.

### Desativando o Fast Boot

O Fast Boot é uma característica específica destes sistemas novos da Microsoft.
Quando o usuário desliga o computador, na verdade ele entra em um tipo de
hibernação especial, que faz o tempo de inicialização ser bem menor quando o
computador é ligado novamente. Porém, com essa opção ativada não é possível
entrar na BIOS do PC, pois o SO já entra direto, pulando a etapa do boot que
permite acessar as configurações do sistema.

Para desativar o Fast Boot, siga os seguintes passos:

1. Localize o ícone da bateria na área de notificações da barra de tarefas.
   Clique com o botão direito no ícone e selecione **Opções de Energia**
2. Nas Opções de Energia, no lado esquerdo da tela, selecione **Escolher a
   função do fechamento da tampa**
3. Na parte superior da tela, selecione **Alterar configurações não disponíveis
   no momento**
4. Na parte inferior da tela, desmarque a caixa de seleção **Ligar inicialização
   rápida**

Agora, basta reiniciar o computador e apertar a tecla específica para entrar na
BIOS do computador (normalmente é `F2`, mas pode ser `Del`, `F4`, `F8`,
dependendo do fabricante).

Após entrar na BIOS, podemos desativar a segunda opção necessária para realizar
o dual boot.

### Desativando o Secure Boot

Outra característica dos computadores novos (que possuem UEFI) é o Secure Boot.
Com ele ativado, o firmware do PC não deixa sistemas não autorizados pela
Microsoft inicializarem na máquina, dentre outras restrições. Por isso, também
é importante desativá-lo.

Algumas montadoras, como a Acer, impedem que o Secure Boot seja desativado caso
o computador não tenha a senha de supervisor setada na BIOS.

#### Notebooks Acer

Para desativar o Secure Boot em notebooks Acer, siga os seguintes passos:

1. Tendo desativado o Fast Boot, acesse a BIOS apertando `F2` durante a
   inicialização.
2. Ao entrar na BIOS, acesse a aba **Security** e aperte `Enter` em **Set
   Supervisor Password**.
3. Após criada a senha, acesse a aba **Boot**, aperte `Enter` em **Secure
   Boot** e selecione **Disabled**.

#### Notebooks de outras marcas

Geralmente, o processo é bem parecido com as instruções acima, exceto pela
necessidade de setar uma senha de supervisor. Em outras palavras, basta
executar o passo 3, acima.

#### Grub quebrado ou não reconhecendo o windows

No Ubuntu a ferramenta *boot-repair* pode ser usada para reparar o grub.

#### Notebooks que bootam o windows após a instalação

Ver *Grub quebrado ou não reconhecendo o windows* acima.

Há firmwares EFI que podem não aceitar um caminho de boot direfente do Windows. Nesse caso pode ser tentado usar a carta na manga da figura photo_2018-09-04_22-01-40.png presente nesse repositório
