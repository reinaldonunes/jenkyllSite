---
layout: post
title:  "Até que enfim, Windows Terminal"
date:   2021-12-13 22:40:35 -0300
categories: jekyll update
image: "https://store-images.s-microsoft.com/image/apps.64156.13926773940052066.16e93a5b-b25f-4aaf-8a38-77375e237879.00013886-8351-473f-9acd-7fcce9ee7388?w=1399&h=792&q=90&format=jpg"

---
# ATÉ QUE ENFIM, WINDOWS TERMINAL

Se você está acostumado a usar *CLIs - Command Line Interface*, ou *terminal de comando* em sistemas baseados em Linux ou Mac, certamente já encontrou dificuldades em usar o *CMD* do Windows. 

Essa "dificuldade" era sempre resolvida com alternativas de terceiros, como o *Hyper.js* e o *CMDER*. Porém, agora com o **Windows Terminal**, é possível utilizar várias CLIs num mesmo programa, além de poder obter uma experiência extremamente melhor.

### INSTALAÇÃO E CONFIGURAÇÃO
Antes de mais nada, se você não possui o programa, precisa acessar a *Microsoft Store* e baixar o Terminal por lá. Ou se preferir, acesse:
- [Microsoft Store](https://www.microsoft.com/pt-br/p/windows-terminal/9n0dx20hk701?activetab=pivot:overviewtab)
- [GitHub](https://github.com/microsoft/terminal)
<br /><br />
Após isso, para poder executar algumas customizações, é necessário modificar as *políticas de execução do Power Shell*. Para isso, procure no Iniciar pelo programa Power Shell e execute em modo administrador.

Após isso, insira o seguinte comando:
```
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned
```

Com isso, você está autorizando o Power Shell a instalar programas e recursos de outras fontes. Basta fechar a janela e reabrir o programa que já estará em vigor a nova política de execução.

### CUSTOMIZAÇÃO PADRÃO
Se você não quer mudar muida coisa no terminal, pode utilizar as customizações padrões do sistema. Para isso, pressione ``CTRL + ,`` para abrir a janela de configuração. 

Nela você poderá alterar desde a forma como o programa inicializa (em tela cheia, padrão, foco, etc) até cores e fontes.

![Configuração Padrão do Windows Terminal](https://i.ibb.co/pnC8HkK/terminal-padrao.png)


### POSH-GIT E OH-MY-POSH
Agora, se você quer deixar o seu terminal radicalmente diferente, para isso vamos utilizar dois módulos extras. 
```
Install-Module posh-git -Scope CurrentUser
Install-Module oh-my-posh -Scope CurrentUse
```
O **Posh-git** vai nos trazer informações sobre o repositório atual, enquanto o **Oh-My-Posh** vai tratar de customizar a aparência do terminal, deixando-a mais bonita.

![Exemplo do terminal com Oh-My-Posh](https://i.ibb.co/vwkhwg1/terminal-new.png)

Após instalar os módulos adicionais, agora é necessário configurar o arquivo de inicialização do Terminal.
> É necessário ter o VS Code instalado para executar essa parte.
No terminal, digite ``code $PROFILE``

Depois, substitua qualquer texto que houver por este:
```
Import-Module posh-git
Import-Module oh-my-posh
Set-PoshPrompt Material
```

Salve, feche e reinicie as janelas do Terminal. Pronto! Já temos o novo visual configurado!

> Caso queira alterar o tema, basta acessar essa [lista aqui](https://github.com/JanDeDobbeleer/oh-my-posh) e trocar o *Material* pelo nome do novo tema. Por exemplo: *Avit*, *Zash*, *TonyBaloney*, etc.

### RECOMENDAÇÕES
Para a configuração ficar o mais perfeita possível, recomenda-se utilizar a tipografia *Cascadia*, *Source Code Pro* ou *Fira Mono*.
