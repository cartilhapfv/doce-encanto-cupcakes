# Organização e armazenamento de dados — Doce Encanto

## Modelo simplificado implementado
O protótipo registra os seguintes dados para cada pedido:

| Campo | Descrição |
|---|---|
| nome_cliente | Nome informado pelo cliente |
| endereco_cliente | Endereço informado para entrega |
| sabor | Um sabor selecionado |
| quantidade | Quantidade de unidades |
| total | Valor calculado do pedido |

Os preços são fixos: Chocolate Gourmet = R$ 9,00; Morango = R$ 10,00; Red Velvet = R$ 11,00. O total corresponde ao preço unitário multiplicado pela quantidade.

## Versão original
O aplicativo Android utiliza o componente **TinyDB** para armazenar informações localmente. A versão web original mantém uma representação do último pedido no armazenamento local do navegador.

## Versão melhorada
- **Android:** lista de pedidos anteriores mantida em variável e salva no TinyDB sob a etiqueta `historico_pedidos`, para recuperação quando a tela é iniciada.
- **Web:** pedidos salvos em uma lista JSON no `localStorage`, com data de registro e os dados do pedido. O histórico é exibido na própria página.
- **Limpar formulário:** redefine os campos visíveis, sem excluir os pedidos armazenados.

## Limitações
Não existe banco de dados remoto, conta de usuário, integração de pagamento ou sincronização. Os dados ficam restritos ao aplicativo/dispositivo ou ao navegador usado. A limpeza dos dados do aplicativo ou do navegador pode eliminar os registros locais.

Este documento descreve a organização de dados do protótipo, não um banco de dados relacional implementado.
