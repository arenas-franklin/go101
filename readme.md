# GO LANG 101

Documentação:   https://go.dev/


## O que é a Go Lang?

- Linguagem de programação open souce que tem o objetivo de tornar os programadores mais produtivos
- Expressiva, concisa, limpa e eficiente
- Foi criada para aproveitar ao máximo dos recursos multicore e de rede
- Rápida compilaão e ao mesmo tempo travalha com garbage collection
- Rápida, estaticamente tipada, compilada mas que ao mesmo tempi parece até uma lingugam dinamicamente tirada e interpretada.
- Compilada apenas um arquivo binário

## Aonde Nasceu e quem criou?

- Google
- Projeto incial em 2007 -Set
- Versão 1.0; 2012
- 1.5 Linguagem reescreveu seu compilador em GO
- Robert Giesemar - V8
- Rob Pike - UNIX & UTF-8
- Ken Thompson - UNIX & UTF-8

## Por que uma nova linguagem? Por que GO?

- Limitações algumas das principais llingugaem utilizadas na Google como Python, Java e C++
- Python: probrlma com lentidão
- C/C++: Muita Complecidade e demorado para coliplar
- Java: Complexidade gerada ao longo do tempo/ verbosidade da lingugaem
- Multitheading e Concorrência: Não nasceram nativamente pensando nisso;
- Simplicidade
- Framework de teste e profiling nativos
- Detecção de rece conditions
- Deploy absurdamente simples
- Baixa curva de aprendizado

para rodar o programa 
```go lang
    go run nome-programa.go

// ou 

    go run .
```

para criar umarquivo binário
```go lang
    go build nome-programa.go
```

**Chamar pacote externo**

pesquisar o pacotedesejando no site:
https://pkg.go.dev/

adiciona o pacote no seu arquivo

```go lang
package main

import "fmt"

import "rsc.io/quote"

func main() {
    fmt.Println(quote.Go())
}
```

adicone o novo mod requerido e sum com seguinte comando no terminal:

```go lang
    go mod tidy
```