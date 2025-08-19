# Distro-Linux

Projeto baseado no livro Linux From Scratch (LFS). Este repositório contém as fontes XML, scripts e estilos necessários para gerar o livro em múltiplos formatos (HTML chunked/nochunks e PDF), além de artefatos auxiliares.

## Como construir

Pré-requisitos: consulte o arquivo `INSTALL` para instalar as dependências.

- Compilar para HTML (chunked):
  - `make BASEDIR=/caminho/para/saida`
- Compilar para HTML em arquivo único (nochunks):
  - `make BASEDIR=/caminho/para/saida nochunks`
- Compilar para PDF:
  - `make BASEDIR=/caminho/para/saida pdf`

Observação: para gerar a versão com systemd, defina a variável `REV=systemd` (ex.: `make REV=systemd BASEDIR=...`).

## Estrutura

- `chapter01..11/`: capítulos do livro em XML
- `stylesheets/`: XSL e CSS para renderização
- `bootscripts/` e `udev-lfs/`: recursos e scripts auxiliares
- `chapter10/kernel/`: arquivos e scripts de configuração do kernel

## Licenciamento

Ver `appendices/license.xml` e `appendices/mit-lic.xml`.