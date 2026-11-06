# Requisitos e evolução funcional — Doce Encanto

## Contexto
O projeto começou no PIT I como proposta de aplicativo para uma loja fictícia de cupcakes gourmet. A versão implementada concentra-se no registro simples de pedidos. Pagamento online, gestão de entregas e carrinho com vários sabores não integram o protótipo atual.

## Requisitos da versão original
| Código | Requisito | Situação |
|---|---|---|
| RF01 | Exibir opções de cupcakes e respectivos preços | Implementado |
| RF02 | Selecionar um sabor por pedido | Implementado |
| RF03 | Informar nome e endereço do cliente | Implementado |
| RF04 | Informar quantidade desejada | Implementado |
| RF05 | Calcular o total conforme sabor e quantidade | Implementado |
| RF06 | Registrar e confirmar o pedido | Implementado |

Sabores e preços utilizados: Chocolate Gourmet (R$ 9,00), Morango (R$ 10,00) e Red Velvet (R$ 11,00).

## Melhorias do PIT II
| Código | Melhoria | Descrição |
|---|---|---|
| RF07 | Histórico de pedidos | Consultar registros anteriores, com cliente, endereço, sabor, quantidade e valor |
| RF08 | Limpar formulário | Apagar os campos do formulário e redefinir o valor exibido, sem apagar o histórico |

As duas melhorias foram incorporadas à lógica do projeto Android e à demonstração web melhorada. O histórico do Android utiliza TinyDB; o histórico web utiliza localStorage, ambos locais.

## Requisitos não funcionais
- Interface simples e compreensível.
- Cálculo claro do total.
- Organização dos dados de pedido.
- Armazenamento local, sem necessidade de servidor.
- Funcionamento voltado à demonstração acadêmica.

## Fluxo básico
1. Escolher um sabor.
2. Informar nome, endereço e quantidade.
3. Calcular o valor total.
4. Registrar o pedido e visualizar a confirmação.
5. Na versão melhorada, consultar o histórico ou limpar os campos.

## Restrições e validação
- Um sabor por pedido.
- Sem pagamentos ou entregas reais.
- Sem sincronização ou banco de dados remoto.
- A implementação documentada não equivale a teste funcional concluído. Resultados de execução dos APKs no Appetize.io devem ser registrados após a realização dos testes.
