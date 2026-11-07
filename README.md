# Sistema de Cadastro de Compras em C

Programa em C com interface gráfica (Win32 / `windows.h`) para cadastrar compras
e consultá-las. Desenvolvido para o trabalho de Programação de Software Básico em C.

## Funcionalidades

- **Salvar compra:** valida produto, quantidade e preço, calcula o total
  (`quantidade * preço`) e grava a linha `produto;quantidade;preço;total` em `aval1234.txt`.
- **Mostrar compras:** lê o arquivo, lista todas as compras na tela e exibe o
  total geral e o número de compras.
- **Limpar:** limpa os campos e a lista.

## Como compilar

Requer Windows e um compilador GCC (MinGW), por exemplo o Code::Blocks com MinGW.

```
gcc main.c -o cadastro.exe -mwindows
```

No Code::Blocks: crie um projeto, cole o código em `main.c`, adicione `-mwindows`
em *Project > Build options > Linker settings > Other linker options* e aperte F9.

## Formato do arquivo `aval1234.txt`

```
Teclado;2;100.00;200.00
Mouse;3;50.00;150.00
```

## Arquivos

- `main.c`: código-fonte completo.
