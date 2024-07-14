# ft_printf

Este repositório contém a implementação do projeto `ft_printf` da 42. O objetivo do projeto é recriar a função `printf` da biblioteca padrão C, que é usada para a formatação e impressão de dados.

## Índice

- [Sobre](#sobre)
- [Funcionalidades](#funcionalidades)
- [Como Usar](#como-usar)
- [Instalação](#instalação)
- [Exemplos de Uso](#exemplos-de-uso)
- [Compilação do Projeto](#compilação-do-projeto)
- [Créditos](#créditos)

## Sobre

O projeto `ft_printf` visa entender profundamente a função `printf`, suas complexidades e como implementar uma função de formatação personalizada em C. Este projeto é parte do currículo da escola 42.

## Funcionalidades

A implementação de `ft_printf` suporta:

- Caracteres (`%c`)
- Strings (`%s`)
- Ponteiros (`%p`)
- Números inteiros (`%d`, `%i`)
- Números inteiros não sinalizados (`%u`)
- Números hexadecimais (`%x`, `%X`)
- O caractere de porcentagem (`%%`)

## Como Usar

Para usar a função `ft_printf` em seu projeto, você precisa incluir o cabeçalho `ft_printf.h` e compilar o arquivo fonte `ft_printf.c` com seu projeto.

```c
#include "ft_printf.h"

int main(void)
{
    ft_printf("Hello, %s!\n", "cefelix");
    return 0;
}
```

## Instalação

1. Clone o repositório:

   ```sh
   git clone https://github.com/seu-usuario/ft_printf.git
   cd ft_printf
   ```

2. Compile a biblioteca:

   ```sh
   make
   ```

3. Inclua a biblioteca `libftprintf.a` e o cabeçalho `ft_printf.h` em seu projeto.

## Exemplos de Uso

```c
#include "ft_printf.h"

int main(void)
{
    int num = 42;
    char *str = "cefelix";
    ft_printf("Hello, %s!\n", str);
    ft_printf("The answer is %d\n", num);
    ft_printf("Memory address: %p\n", &num);
    ft_printf("Hexadecimal: %x\n", num);
    return 0;
}
```

Saída esperada:

```
Hello, cefelix!
The answer is 42
Memory address: 0x7ffee6b8e5dc
Hexadecimal: 2a
```

## Compilação do Projeto

Para compilar o seu projeto com a biblioteca `ft_printf`, siga os passos abaixo:

1. Certifique-se de que a biblioteca `libftprintf.a` e o cabeçalho `ft_printf.h` estão no mesmo diretório que seu arquivo de código fonte, ou ajuste os caminhos conforme necessário.

2. Compile seu arquivo de código fonte junto com a biblioteca `ft_printf`. Aqui está um exemplo de como fazer isso usando `gcc`:

   ```sh
   gcc -o meu_programa main.c libftprintf.a
   ```

3. Execute o programa:

   ```sh
   ./meu_programa
   ```

## Créditos

Este projeto foi realizado como parte do currículo da [42Luanda](https://42luanda.com/), uma rede global de escolas de programação.

![imagem do codigo fonte:](printf_image1.png)
![imagem do resultado dos testes funcionais:](printf_image2.png)
