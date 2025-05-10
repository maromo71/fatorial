## Visualização de Fatorial com Pilha de Chamadas
Este é um aplicativo web interativo que visualiza o cálculo do fatorial de um número e a manipulação da pilha de chamadas durante o processo. Ele foi desenvolvido para ajudar a entender como a recursão funciona e como a pilha de chamadas é usada para gerenciar as chamadas de função.

### Funcionalidades
**Entrada de Número:** Permite que o usuário insira um número inteiro não negativo para calcular o fatorial.
**Visualização da Pilha de Chamadas:** Exibe a pilha de chamadas em tempo real, mostrando as chamadas de função e os retornos.
**Animação Passo a Passo:** Destaca a linha de código C correspondente à etapa atual da execução, com um delay para facilitar a compreensão.
**Explicação do Código C:** Fornece o código C da função fatorial recursiva e explica como a pilha de chamadas é usada no processo.
**Interface Interativa:** A interface do usuário é intuitiva e fácil de usar, com estilos claros e concisos.

### Como Usar
1. Clone ou baixe este repositório.
2. Abra o arquivo index.html em seu navegador web.
3. Digite um número inteiro não negativo no campo de entrada.
4. Clique no botão "Calcular Fatorial".
5. Observe a visualização da pilha de chamadas e os passos da depuração.

### Tecnologias Usadas
* HTML
* CSS (Tailwind CSS)
* JavaScript

### Explicação do Código C
O aplicativo visualiza a execução do seguinte código C:

```C
int fatorial(int n) {
    if (n == 0) {
        return 1;
    } else {
        return n * fatorial(n - 1);
    }
}
```

A função fatorial é implementada recursivamente. Para cada chamada da função, um novo quadro é adicionado à pilha de chamadas. O quadro contém as variáveis locais da função e o endereço de retorno. Quando o caso base (n == 0) é atingido, a função retorna 1, e os quadros da pilha são desempilhados à medida que as chamadas recursivas retornam.

### Visualização da Pilha de Chamadas
A pilha de chamadas é visualizada como uma lista. Cada item da lista representa um quadro na pilha. Um quadro pode ser uma chamada de função ou um retorno de função.

**Chamada de função:** Quando a função fatorial é chamada, um novo quadro é adicionado ao topo da pilha. O quadro contém o valor de n para a chamada da função e o endereço de memória da chamada da função.
**Retorno de função:** Quando uma chamada de função retorna, o quadro correspondente é removido da pilha. O valor retornado pela função é exibido no quadro de retorno.
#### Passos da Depuração
A seção "Passos da Depuração" exibe a sequência de chamadas de função e retornos que ocorrem durante o cálculo do fatorial. Para cada passo, o valor de n, o endereço de memória e a ação realizada são exibidos. A linha de código C correspondente à etapa atual da execução é destacada no código C.

### Requisitos
Navegador web moderno com suporte a JavaScript.

### Contribuição
Contribuições são bem-vindas! Se você encontrar algum problema ou tiver alguma sugestão de melhoria, sinta-se à vontade para abrir uma issue ou enviar um pull request.