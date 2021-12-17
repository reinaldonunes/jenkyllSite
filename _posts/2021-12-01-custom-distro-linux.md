---
layout: post
title:  "Como customizar sua distro Linux?"
date:   2021-12-16 22:40:35 -0300
categories: jekyll update
image: "https://sempreupdate.com.br/wp-content/uploads/2020/09/touch.jpg"
---

Sem dúvida, a customização do seu sistema operacional diz muito sobre sua personalidade, seu workflow e seus gostos. Apesar de sistemas como Windows possibilitarem customizações, de longe as realizadas em distros Linux são as melhores e mais fáceis, ao meu ver, de serem realizadas.

> Para estas dicas, foi utilizado o sistema Zorin Core 16, baseado no Ubuntu 20.04 LTS e com DE Gnome 3.38.

# CUSTOMIZAÇÃO PADRÃO
Todo sistema operacional possui no menu Configurações, uma parte dedicada a customização padrão da interface. No caso do Zorin, há o aplicativo Zorin Appearence, que nos permite modificar a forma de apresentação do workflow, o tema de cores, configurações dos ícones e também das fontes. Particularmente, gosto do tema de cores Dark e do layout Gnome, com todos os aplicativos disponíveis (como na foto abaixo)

![Tela de apresentação do Zorin Appearence](https://raw.githubusercontent.com/reinaldonunes/CustomizeDistroLinux/main/assets/customize-img-01.png)

### PLANO DE FUNDO
Mudar a imagem de fundo padrão da sua distro Linux também pode ser uma tarefa fácil. Indo nas configurações padrões do sistema ou **clique da direita - alterar fundo** já será possível escolher outra imagem. Você poderá optar pelas imagens que o sistema fornece ou mesmo selecionar a sua foto preferida.

![Configurando e alterando o plano de fundo](https://raw.githubusercontent.com/reinaldonunes/CustomizeDistroLinux/main/assets/customize-img-02.png)

# ADICIONANDO UMA DOCK
Distros como o Ubuntu tem uma dock lateral, mas com pouca personalização nativa, o que pode dificultar um pouco se você for iniciante no sistema. Porém, há outras distros baseada em Ubuntu que possibilitam uma maior customização desse recurso, como o **Elementary OS** ou **Fenix OS**, onde a dock fica localizada na parte inferior e possui mais opções de customização.

Caso a sua distro não tenha uma dock nativa (como é o caso do Zorin OS), há algumas formas de você adicionar ela ao sistema.

### APLICANDO A EXTENSÃO DASH TO DOCK
Há uma extensão para o ambiente GNOME disponível no site [Gnome Extensions](https://extensions.gnome.org/extension/307/dash-to-dock/).  Primeiramente, se você não tiver uma extensão GNOME instalada no seu browser, o site irá notificar e solicitar a instalação. Após terminar a instalação no browser, basta recarregar a página e clicar no botão **ON/OFF**, para ligar ou desligar a dock. Após ligar ela, basta personalizar como desejar.

![Adicionando a extensão Dash to Dock via browser](https://raw.githubusercontent.com/reinaldonunes/CustomizeDistroLinux/main/assets/customize-img-03.png)

### PLANK DOCK
Mas se você preferir uma dock mais elegante e prática, pode então optar por instalar o Plank. O plank cria uma dock integrada no seu sistema, podendo ser facilmente personalizada e customizada, desde aparência, comportamento e também posição.

![Plank dock](https://raw.githubusercontent.com/reinaldonunes/CustomizeDistroLinux/main/assets/customize-img-04.png)

Para instalar, há duas formas:
- [x] Abrindo a sua central de programas (ou loja de aplicativos), procure por Plank, depois clique em instalar, aguarde completar e pronto!

- [x] No terminal, digite:
```
sudo add-apt-repository -y ppa:ricotz/docky
sudo apt-get update
sudo apt-get install plank
```
Com isso, o Plank será instalado corretamente.

> Se você não gostar do Plank, pode desinstalá-lo via loja de aplicativos ou pelo terminal com `sudo apt-get remove plank --auto-remove`.


# APLICANDO TEMAS DE TERCEIROS
Há também outras formas de customizar a sua distro que é através de sites como o [DeviantArt](https://www.deviantart.com/) e o [Gnome-Look](https://www.gnome-look.org/s/Gnome/browse/). Neles, é possível baixar diversos temas de desktop, icones, grub, entre outros.

1. Acesse o site do Gnome-Looks e pesquiser por algum tema de seu gosto (como MacOs, Fluent, Rounded Theme, etc).
2. Clique no botão Download. Vai aparecer uma lista de pacotes para você escolher e baixar. Clique sobre algum do seu gosto.
3. Na caixa de diálogo que abrir, clique novamentem em Download e aguarde.
4. Na próxima janela que abrir, marque a opção *Abrir* e depois clique em *Ok*.
5. Irá aparecer os itens internos do pacote. Clique me *Extrair*. 
6. Vai aparecer as pastas do seu sistema. Pressione *CTRL+H* para exibir as pastas ocultas e encontre a que se chama *.themes*. Se não existir, você mesmo poderá criá-la.
7. Dentro da pasta .themes, clique no botão *extrair* para baixar completamente o tema.
8. Após baixado, basta ir nas configurações padrões do seu sistema e selecionar o tema que foi baixado (veja a primeira seção deste tutorial).

![Capturas do passo a passo do tema](https://raw.githubusercontent.com/reinaldonunes/CustomizeDistroLinux/main/assets/customize-img-05.png)

### USANDO O GNOME-TWEAKS COMO AUXILIAR
Além dessas opções, você também pode instalar e utilizar o *Gnome Tweaks* ou *Ajustes do Gnome* para ter ainda mais poder de configuração e customização na sua distro. Basta abrir a loja de aplicativos e pesquisar por um dos termos mencionados anteriormente para poder utilizá-lo na máquina.

![Gnome-Tweaks](https://raw.githubusercontent.com/reinaldonunes/CustomizeDistroLinux/main/assets/customize-img-06.png)

Se prefir, também poderá instalar a ferramenta via terminal. Primeiro, atualize o APT com `sudo apt update` e depois instale digitando `sudo apt install gnome-tweaks` colocar sua senha root e aguardar.


# INSTALANDO TEMAS VIA TERMINAL
Se você quiser se aventurar mais pelo Linux, poderá fazer customizações diretas via terminal. Na internet é possível encontrar diversos sites que orientam como fazer, já que cada tema terá seu método específico de ser instalado. Para saber mais, recomendo ler este post do site **[Viva o Linux](https://www.vivaolinux.com.br/dica/Como-instalar-temas-no-Ubuntu-1110)**, a maior comunidade de usuários GNU/Linux da América Latina.
