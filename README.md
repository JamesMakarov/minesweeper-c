# Minesweeper in C

[![C build](https://github.com/JamesMakarov/minesweeper-c/actions/workflows/ci.yml/badge.svg)](https://github.com/JamesMakarov/minesweeper-c/actions/workflows/ci.yml)

Implementação de **Campo Minado em C**, desenvolvida como projeto acadêmico com separação entre a lógica do jogo e a camada de interface.

## Funcionalidades

- geração dinâmica do tabuleiro;
- distribuição de minas;
- contagem de minas vizinhas;
- abertura recursiva de células;
- marcação e remoção de bandeiras;
- verificação de vitória e derrota;
- sistema de dica;
- configuração de dimensões e quantidade de minas.

## Estrutura

```text
src/
├── back/
│   ├── campominado.c
│   └── campominado.h
├── interface/
│   ├── interface.c
│   └── interface.h
└── main.c
```

A estrutura `Celula` mantém referências para as células vizinhas, enquanto `Tabuleiro` gerencia a matriz de células e o estado global da partida.

## Compilação

### Linux / macOS

Com GCC e Make instalados:

```bash
make
./campominado
```

Ou:

```bash
make run
```

Também há o script:

```bash
./jogar_Linux_MacOS.sh
```

### Windows

Use o script:

```bat
jogar.bat
```

ou compile manualmente com GCC/MinGW.

## Colaboração

Projeto desenvolvido em equipe:

- **Samuel Dantas de Carvalho** — participação principal no sistema de dica.
- **Thiago Monteiro Nogueira** — participação principal na lógica do jogo.
- **Vitor Nogueira de Sousa** — participação principal na interface.

Todos os integrantes também contribuíram na integração e correção de erros.
