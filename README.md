# UFLA-RISC | Simulador de Processador 32 bits

Simulador funcional desenvolvido em **Python** para interpretação e execução de instruções da arquitetura **UFLA-RISC de 32 bits**.

O projeto reproduz o funcionamento de um processador hipotético, desde a tradução de programas Assembly para código binário até a execução das instruções, incluindo operações sobre registradores e memória.

Desenvolvido em equipe durante a disciplina de **Arquitetura de Computadores II**, na Universidade Federal de Lavras (UFLA), como aplicação prática de conceitos de arquitetura de processadores e programação de baixo nível.

---

## Visão Geral

O simulador implementa a arquitetura UFLA-RISC, permitindo carregar e executar programas escritos para seu conjunto de instruções (ISA).

O processo envolve:

- **Montagem:** conversão de instruções Assembly (`.asm`) em código binário (`.bin`).
- **Busca e decodificação:** leitura e interpretação das instruções do programa.
- **Execução:** processamento das operações e atualização dos registradores e da memória.
- **Acompanhamento:** exibição de logs de execução e do estado final do processador.

## Tecnologias

- **Python**
- **Assembly**
- **Arquitetura RISC de 32 bits**

## Como Executar

### Pré-requisitos

- Python instalado.

### 1. Clone o repositório

```bash
git clone https://github.com/lanamiranda17/ufla-risc-simulador-grupo-2.git
cd ufla-risc-simulador-grupo-2
```

### 2. Prepare o programa Assembly

Abra o arquivo `src/interpretador/programa.asm` e substitua seu conteúdo pelo código Assembly que deseja executar.

O diretório `src/testes/testes_assembly` contém exemplos de programas `.asm` que podem ser utilizados para testar o simulador.

**Nota:** o simulador utiliza `programa.asm` como arquivo de entrada padrão.

### 3. Execute o simulador

Na raiz do projeto, execute:

```bash
python src/main.py
```

### 4. Verifique os resultados

O terminal apresentará:

- Confirmação da conversão de Assembly (`.asm`) para binário (`.bin`).
- Logs da execução das instruções, incluindo as etapas de busca e decodificação (Fetch/Decode).
- Estado final dos registradores e da memória.

### Exemplo de execução

Saída do simulador utilizando o programa `teste_sub.asm`:

<img width="1302" height="831" alt="Exemplo de execução do simulador UFLA-RISC" src="https://github.com/user-attachments/assets/b0a4c1a7-5765-4ca0-9390-d88b5795c507" />

---

## Equipe de Desenvolvimento

- Lana da Silva Miranda
- Fábio Damas Valim
- Guilherme Lirio Miranda
- Marcos Vinícius Pereira
- Arthur Soares Marques

**Universidade Federal de Lavras (UFLA)**  
Disciplina: Arquitetura de Computadores II
