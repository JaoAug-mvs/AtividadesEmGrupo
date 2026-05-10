# ihcux-racha-ai-blazor

Projeto desenvolvido para a disciplina de Interação Humano Computador e UX do Centro Universitário UNA.

O objetivo da atividade foi transformar um wireframe criado no Miro em uma interface funcional utilizando Blazor com C#/.NET, aplicando conceitos de UX, hierarquia visual, responsividade e componentização.

---

## Integrantes

- Pedro Morais Hilbert  
- Letícia Petrina Machado Silva  
- Daniel de Almeida Vieira  
- João Augusto Miranda Viana de Souza  
- Luana Xaviel Monteiro  

---

# Sobre o Projeto

O projeto simula o dashboard principal do aplicativo fictício **RachaAí**, uma plataforma voltada para divisão de despesas em grupo.

A interface foi pensada para mostrar rapidamente:
- quanto o usuário tem a receber;
- quanto ele precisa pagar;
- e o saldo geral.

Além disso, o dashboard apresenta os grupos ativos em cards reutilizáveis criados com componentes Blazor.

---

# Implementação Blazor

Durante o desenvolvimento, a principal preocupação foi manter a organização visual do wireframe original e transformar isso em componentes reutilizáveis.

Os cards superiores foram usados para destacar informações importantes logo no primeiro contato com a tela, utilizando cores para facilitar a leitura:
- verde para valores positivos;
- vermelho para despesas;
- e tons neutros para informações gerais.

A listagem de grupos foi separada em um componente próprio chamado `GrupoCard`, permitindo reutilização de código e deixando a página principal mais limpa e organizada.

Também utilizamos o sistema de Grid do Bootstrap para garantir responsividade em diferentes tamanhos de tela.

---

# Estrutura do Projeto

```plaintext
Models/
 └── Grupo.cs

Shared/
 └── GrupoCard.razor

Pages/
 └── Dashboard.razor
