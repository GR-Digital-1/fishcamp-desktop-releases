# Fishcamp para Windows e Linux

Instaladores do app de computador do [Fishcamp](https://fishcamp.space). Este repositório guarda só os arquivos de
cada versão (aba **Releases**). O código fica no repositório privado do produto.

## Baixar

Abra a [versão mais recente](https://github.com/GR-Digital-1/fishcamp-desktop-releases/releases/latest) e baixe o
arquivo do seu sistema:

| Sistema | Arquivo | Como instalar |
|---|---|---|
| Windows 10 e 11 | `Fishcamp-Setup-<versão>.exe` | Abra o arquivo. Ele instala sozinho, sem pedir senha de administrador. |
| Ubuntu, Debian e derivados | `fishcamp_<versão>_amd64.deb` | `sudo apt install ./fishcamp_<versão>_amd64.deb` |
| Outras distribuições Linux | `Fishcamp-<versão>.AppImage` | `chmod +x Fishcamp-*.AppImage` e abra. Pode precisar do pacote `libfuse2`. |

No Windows, enquanto o instalador não for assinado, o aviso "O Windows protegeu o computador" aparece na primeira
vez. Clique em **Mais informações** → **Executar assim mesmo**.

## Depois de instalar

- **Fechar a janela não fecha o app.** Ele continua no ícone perto do relógio, avisando de menções e mantendo a
  chamada. Para sair, use **Sair do Fishcamp** no menu desse ícone.
- **Abre com o computador.** Para desligar, desmarque **Abrir ao iniciar o computador** no mesmo menu.
- **Entrar com o Google:** o app abre o navegador; depois de entrar, clique em **Abrir o Fishcamp**. No AppImage, use
  o código por e-mail.
- **Atualiza sozinho.** O app confere as versões novas daqui e as instala ao sair. No `.deb`, a atualização é pelo
  menu do ícone e pede a senha do sistema.

## Para quem mantém

As versões são publicadas pelo workflow `release-desktop.yml` do repositório do produto, ao criar a tag
`desktop-v<versão>`. Não publique arquivos à mão aqui: o atualizador do app lê os `latest*.yml` gerados pelo build.
