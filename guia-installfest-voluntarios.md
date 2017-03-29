# Guia da installfest para voluntários

Ser voluntário em um installfest é uma tarefa difícil e que demanda
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
de um sistema; o objetivo é ensinar, para que os novos usuários possam um dia
serem também voluntários.

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

**Em construção.**
