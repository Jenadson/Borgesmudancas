# Estrutura da Pagina de Referencia

Referencia analisada: `https://hously1.webflow.io/`

Observacao: a pagina foi usada apenas como inspiracao estrutural. Textos, imagens, marca, estilo proprietario e codigo da referencia nao foram copiados.

## HTML
- Secoes principais:
  - Header fixo/limpo com logotipo, navegacao e CTA.
  - Hero section com chamada principal, texto de apoio, botoes e composicao visual com imagens.
  - Faixa de indicadores/logotipos para transmitir confianca.
  - Secao de categorias/servicos em cards.
  - Bloco de beneficios com lista visual e imagem de apoio.
  - Secao de processo ou etapas.
  - Depoimentos/provas sociais.
  - FAQ em acordeao.
  - CTA final antes do rodape.
  - Footer com colunas de links e contatos.
- Componentes:
  - Botao principal destacado.
  - Botao secundario/outline.
  - Cards com icones.
  - Imagens em composicao assimetrica.
  - Tags/selos de credibilidade.
  - FAQ interativo.
- Hierarquia:
  - Hero com maior peso visual.
  - Conteudo dividido em blocos curtos e escaneaveis.
  - CTAs repetidos em pontos decisivos.

## CSS
- Sistema de cores:
  - Base clara com contraste forte em areas escuras.
  - Cor de destaque usada em botoes e palavras importantes.
  - Neutros para cards e fundos.
- Espacamentos:
  - Secoes amplas em desktop.
  - Grid com largura maxima centralizada.
  - Gaps consistentes entre cards.
- Grid:
  - Hero em duas colunas no desktop.
  - Cards em 3 colunas no desktop.
  - Layout empilhado em telas menores.
- Responsividade:
  - Menu mobile recolhido.
  - Grids convertem para uma coluna.
  - Imagens e botoes ajustam largura.
- Botoes:
  - CTA cheio para acao principal.
  - Outline para acao secundaria.
- Cards:
  - Fundo claro, borda discreta, sombra suave e icone no topo.
- Animacoes:
  - Transicoes leves em hover.
  - Entrada sutil de secoes por classe via JavaScript.

## JavaScript
- Interacoes:
  - Menu mobile abre/fecha.
  - FAQ em acordeao.
  - Atualizacao do ano no rodape.
- Menus:
  - Botao de navegacao mobile com `aria-expanded`.
  - Fechamento do menu apos clique em link.
- Sliders:
  - Nao necessario para a versao final; depoimentos foram mantidos em cards estaticos para melhor desempenho.
- Formularios:
  - CTA direcionado para contato/orcamento; formulario completo pode ser adicionado em etapa posterior.
- Animacoes:
  - Intersection Observer para revelar secoes com movimento suave e acessivel.
