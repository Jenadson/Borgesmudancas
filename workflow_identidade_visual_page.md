# Workflow — Extração de Identidade Visual e Implementação em Página de Referência

## Objetivo

Criar um fluxo automatizado para:

1. Ler todas as imagens dentro da pasta `img`.
2. Extrair a identidade visual usando a skill `skill_identity_extractor`.
3. Criar um arquivo chamado `id_Visual.md` com todas as informações visuais extraídas.
4. Solicitar ao usuário um link de referência.
5. Acessar o link informado.
6. Extrair a estrutura visual, HTML, CSS e JavaScript da página de referência.
7. Recriar/adaptar a página usando a identidade visual extraída no arquivo `id_Visual.md`.
8. Entregar uma página final coerente com a marca do cliente/projeto.

---

## Regras Gerais do Workflow

- Não alterar o logotipo original.
- Não inventar identidade visual se houver imagens suficientes na pasta `img`.
- Usar as imagens como fonte principal de identidade visual.
- O arquivo `id_Visual.md` deve ser criado antes de pedir o link de referência.
- Só pedir o link de referência depois que a análise visual estiver concluída.
- Não copiar textos, marcas, imagens ou código protegido de terceiros sem autorização.
- Usar o link de referência como inspiração estrutural e técnica, não como cópia ilegal.
- Preservar a identidade da marca analisada.
- Manter o projeto organizado.
- Criar backup dos arquivos antes de modificar páginas existentes.

---

## Etapa 1 — Verificar Estrutura do Projeto

Antes de iniciar, verificar se existe a pasta:

```txt
/img
```

A pasta deve conter imagens como:

```txt
logo.png
logo-reduzida.png
fachada.png
camisa.png
veiculo.png
cartao.png
mockup.png
referencias.png
```

Caso a pasta `img` não exista ou esteja vazia, parar o workflow e informar:

```txt
Não encontrei imagens dentro da pasta img. Adicione as imagens da marca nessa pasta para que eu possa extrair a identidade visual.
```

---

## Etapa 2 — Analisar Imagens da Pasta img

Ler todas as imagens presentes na pasta `img`.

Usar a skill:

```txt
skill_identity_extractor
```

A skill deve analisar:

- Logotipo principal
- Logotipo reduzido
- Cores predominantes
- Cores secundárias
- Cores de fundo
- Cores de contraste
- Tipografia aparente
- Estilo visual da marca
- Formas e elementos gráficos
- Estilo de ícones
- Estilo de botões
- Estilo de layout
- Aplicações da marca em mockups
- Atmosfera visual da marca
- Público-alvo sugerido
- Tom visual: moderno, clássico, premium, popular, tecnológico, corporativo etc.

---

## Etapa 3 — Criar o Arquivo id_Visual.md

Após analisar as imagens, criar obrigatoriamente o arquivo:

```txt
id_Visual.md
```

O arquivo deve conter a seguinte estrutura:

```md
# Identidade Visual Extraída

## 1. Nome da Marca

Nome identificado da marca.

---

## 2. Logotipo

Descrição do logotipo principal.

### Logo Principal
- Formato:
- Elementos:
- Cores:
- Estilo:
- Uso recomendado:

### Logo Reduzida
- Formato:
- Elementos:
- Cores:
- Uso recomendado:

---

## 3. Paleta de Cores

### Cores Principais

| Cor | Hexadecimal | Uso recomendado |
|---|---|---|
| Cor 1 | #000000 | Exemplo: fundo, títulos, botões |
| Cor 2 | #FFFFFF | Exemplo: textos, áreas claras |
| Cor 3 | #CCCCCC | Exemplo: detalhes, bordas |

### Cores Secundárias

| Cor | Hexadecimal | Uso recomendado |
|---|---|---|
| Cor 1 | #000000 | Apoio visual |
| Cor 2 | #000000 | Hover, detalhes ou ícones |

---

## 4. Tipografia

### Fonte Principal Sugerida
- Nome ou estilo:
- Peso recomendado:
- Uso:

### Fonte Secundária Sugerida
- Nome ou estilo:
- Uso:

---

## 5. Estilo Visual da Marca

Descrever o estilo geral da marca.

Exemplo:
A marca possui uma identidade visual moderna, limpa e profissional, com forte presença de contraste entre tons escuros e claros. O uso do logotipo deve ser preservado, evitando distorções ou mudanças nas proporções.

---

## 6. Elementos Gráficos

- Bordas:
- Ícones:
- Formas:
- Texturas:
- Padrões:
- Sombras:
- Gradientes:

---

## 7. Direção de Layout

- Tipo de layout recomendado:
- Estilo de hero section:
- Estilo de cards:
- Estilo de botões:
- Estilo de seções:
- Estilo de rodapé:

---

## 8. Aplicação em Website

### Header
- Como usar a logo:
- Cores:
- Menu:
- CTA:

### Hero Section
- Fundo:
- Título:
- Subtítulo:
- Botões:
- Imagem ou mockup:

### Seções Internas
- Cards:
- Ícones:
- Títulos:
- Blocos de conteúdo:

### Footer
- Cores:
- Informações:
- Logo:
- Links:

---

## 9. Regras de Uso

- Não alterar o logotipo.
- Não distorcer proporções.
- Manter contraste adequado.
- Usar a paleta extraída.
- Manter unidade visual em todas as seções.
- Evitar cores fora da identidade visual.

---

## 10. Resumo Final da Identidade

Resumo curto da identidade visual para ser usado como referência rápida.
```

---

## Etapa 4 — Solicitar Link de Referência

Somente depois de criar o arquivo `id_Visual.md`, perguntar ao usuário:

```txt
A identidade visual foi extraída e o arquivo id_Visual.md foi criado. Agora envie o link de referência da página que deseja usar como base estrutural.
```

Aguardar o usuário enviar o link.

---

## Etapa 5 — Acessar o Link de Referência

Após receber o link, acessar a página de referência.

Analisar:

- Estrutura HTML
- Organização das seções
- Header
- Hero section
- Cards
- Serviços
- Seções de benefícios
- Provas sociais
- Galeria
- Formulários
- CTA
- Footer
- Animações
- Responsividade
- Arquivos CSS
- Scripts JavaScript
- Bibliotecas externas utilizadas

---

## Etapa 6 — Extrair Estrutura Técnica

Criar um resumo técnico da página de referência com:

```md
# Estrutura da Página de Referência

## HTML
- Seções principais:
- Componentes:
- Hierarquia:

## CSS
- Sistema de cores:
- Espaçamentos:
- Grid:
- Responsividade:
- Botões:
- Cards:
- Animações:

## JavaScript
- Interações:
- Menus:
- Sliders:
- Formulários:
- Animações:
```

Esse resumo pode ser salvo como:

```txt
referencia_page.md
```

---

## Etapa 7 — Implementar a Identidade Visual na Página

Ler o arquivo:

```txt
id_Visual.md
```

Depois adaptar a página com base nele.

A implementação deve aplicar:

- Paleta de cores extraída
- Tipografia sugerida
- Estilo dos botões
- Estilo dos cards
- Cores de fundo
- Estilo do header
- Estilo do footer
- Logo correta
- Elementos gráficos coerentes
- Responsividade
- Visual moderno e profissional

---

## Etapa 8 — Arquivos Finais Esperados

Dependendo da estrutura do projeto, gerar ou atualizar:

```txt
index.html
style.css
script.js
id_Visual.md
referencia_page.md
```

Caso o projeto use React, gerar ou atualizar:

```txt
src/App.jsx
src/App.css
src/components/
src/assets/
id_Visual.md
referencia_page.md
```

Caso o projeto use Next.js:

```txt
app/page.jsx
app/globals.css
components/
public/
id_Visual.md
referencia_page.md
```

---

## Etapa 9 — Regras de Implementação Visual

A página final deve:

- Ter aparência profissional.
- Parecer feita sob medida para a marca.
- Usar a identidade visual extraída.
- Não parecer uma cópia exata do site de referência.
- Usar o site de referência apenas como base estrutural.
- Ter boa hierarquia visual.
- Ter botões claros e chamativos.
- Ter responsividade para desktop, tablet e mobile.
- Ter código limpo e organizado.
- Ter nomes de classes compreensíveis.

---

## Etapa 10 — Validação Final

Antes de finalizar, conferir:

- O arquivo `id_Visual.md` existe.
- A paleta visual foi aplicada.
- O logo não foi alterado.
- A página está responsiva.
- Não existem erros de HTML.
- Não existem erros de CSS.
- Não existem erros de JavaScript.
- A página funciona no navegador.
- A identidade visual está consistente.
- A página não copiou indevidamente conteúdo protegido do link de referência.

---

## Mensagem Final ao Usuário

Ao terminar, responder:

```txt
Workflow concluído.

Arquivos criados/alterados:
- id_Visual.md
- referencia_page.md
- index.html
- style.css
- script.js

A identidade visual foi extraída das imagens da pasta img e aplicada na página com base na estrutura do link de referência.
```

---

## Comportamento Obrigatório do Agente

O agente deve seguir esta ordem obrigatória:

1. Verificar pasta `img`.
2. Usar `skill_identity_extractor`.
3. Criar `id_Visual.md`.
4. Só depois pedir o link.
5. Acessar o link.
6. Extrair estrutura HTML/CSS/JS.
7. Ler `id_Visual.md`.
8. Implementar a identidade visual na página.
9. Validar resultado.
10. Informar arquivos criados ou alterados.

Nunca pular a criação do `id_Visual.md`.
Nunca pedir o link antes de analisar as imagens.
Nunca alterar o logotipo.

---

# Prompt Curto Para Agente

Você é um agente de desenvolvimento web e identidade visual.

Siga este workflow obrigatoriamente:

1. Analise todas as imagens dentro da pasta img.
2. Use a skill skill_identity_extractor para extrair a identidade visual da marca.
3. Crie um arquivo chamado id_Visual.md com:
   - nome da marca;
   - descrição do logotipo;
   - paleta de cores em hexadecimal;
   - tipografia sugerida;
   - estilo visual;
   - elementos gráficos;
   - regras de uso da marca;
   - recomendações para aplicação em website.

4. Depois de criar o id_Visual.md, pare e solicite ao usuário o link de referência.

Mensagem obrigatória:
"A identidade visual foi extraída e o arquivo id_Visual.md foi criado. Agora envie o link de referência da página que deseja usar como base estrutural."

5. Após receber o link, acesse a página de referência.
6. Extraia a estrutura HTML, CSS e JavaScript da página.
7. Crie um arquivo referencia_page.md resumindo a estrutura da página.
8. Leia o arquivo id_Visual.md.
9. Recrie/adapte a página usando a estrutura do link de referência, mas aplicando a identidade visual extraída das imagens.
10. Não copie conteúdo protegido sem autorização. Use o site apenas como referência estrutural.
11. Não altere o logotipo.
12. Gere ou atualize os arquivos finais do projeto.
13. Valide responsividade, organização do código, aplicação da paleta e funcionamento geral.

Resultado final esperado:
- id_Visual.md
- referencia_page.md
- página implementada com HTML/CSS/JS ou no framework existente do projeto.
