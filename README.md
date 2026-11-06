# Doce Encanto — Cupcakes Gourmet

Projeto acadêmico de Engenharia de Software desenvolvido no PIT I e evoluído no PIT II.

## Objetivo
Aplicativo Android simples para registrar pedidos de cupcakes gourmet, selecionando **um sabor por pedido**, nome do cliente, endereço de entrega e quantidade. O total é calculado conforme o sabor escolhido.

## Versões
- **Versão original (PIT I):** formulário de pedido, seleção de sabor, cálculo do total e confirmação de registro.
- **Versão melhorada (PIT II):** mantém as funções anteriores e acrescenta **histórico de pedidos** e **botão Limpar formulário**. Não foi incluída a seleção de vários sabores no mesmo pedido.

## Tecnologias
- **Aplicativo Android:** MIT App Inventor, com lógica em blocos visuais.
- **Persistência local no aplicativo:** TinyDB.
- **Demonstrações web:** HTML, CSS e JavaScript, publicadas no GitHub Pages; histórico armazenado no navegador por localStorage.
- **Versionamento e documentação:** GitHub.

As páginas web são demonstrações complementares e **não substituem os APKs**. O projeto não processa pagamentos nem envia pedidos reais.

## Demonstrações
- [Site original](https://cartilhapfv.github.io/doce-encanto-cupcakes/)
- [Site melhorado — histórico e limpeza](https://cartilhapfv.github.io/doce-encanto-cupcakes/site-melhorado/)

Os APKs podem ser apresentados em um simulador Android, como o Appetize.io, após o envio dos respectivos arquivos. O uso do simulador não representa, por si só, uma validação de testes concluídos.

## Documentação
- [Requisitos e evolução funcional](docs/requisitos.md)
- [Organização e armazenamento dos dados](docs/modelagem-dados.md)

## Limitações
Armazenamento local, sem sincronização entre dispositivos. A execução do aplicativo, a compatibilidade do APK e os resultados de testes devem ser verificados e registrados separadamente.
