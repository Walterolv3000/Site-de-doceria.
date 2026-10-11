# E de Chocolate Doceria — Website

## Sobre o projeto

Este projeto tem como objetivo criar um website profissional para a **E de Chocolate Doceria**, utilizando como referência principal o perfil oficial da marca no Instagram:

- Instagram: https://www.instagram.com/edechocolatedoceria/

O site deve funcionar como uma extensão digital do Instagram, preservando a identidade visual da doceria, valorizando as fotografias originais dos produtos e facilitando o contato dos clientes para pedidos e encomendas.

> **Importante:** o acesso automatizado ao Instagram pode ser limitado. Utilize somente imagens, textos e informações comerciais disponíveis ou fornecidos pelo proprietário. Não invente produtos, preços, depoimentos, endereço, horários ou outros dados da marca.

## Objetivos

- Preservar a identidade visual original da marca.
- Apresentar os produtos de forma atraente.
- Reutilizar fotografias e textos originais autorizados.
- Facilitar o contato e as encomendas.
- Oferecer uma experiência acessível, responsiva e rápida.
- Criar uma base de código organizada e fácil de manter.

## Referências e conteúdo

Antes da implementação, analisar, quando disponíveis:

- Logotipo e foto do perfil.
- Biografia e informações comerciais.
- Publicações, Reels e fotografias dos produtos.
- Legendas e chamadas comerciais.
- Paleta de cores e tipografia.
- Embalagens, etiquetas e elementos gráficos.
- Canais de atendimento publicados oficialmente.

Se o conteúdo não puder ser acessado, solicitar ao proprietário as fotografias, capturas de tela, legendas, logotipo e dados de contato necessários. Não utilizar fotos de outras docerias como se fossem produtos da marca.

## Design System

O Design System deve ser extraído das referências reais antes do desenvolvimento.

Documentar e padronizar:

- Cores primárias, secundárias e neutras.
- Cores de fundo, superfícies e textos.
- Tipografia, pesos e escala de fontes.
- Espaçamentos e larguras de conteúdo.
- Grid, alinhamentos e proporções.
- Bordas, sombras e border-radius.
- Estilo dos botões, links e formulários.
- Tratamento, enquadramento e proporções das imagens.
- Estados de foco, hover e interação.

Utilizar variáveis CSS para centralizar os tokens. Não escolher cores, fontes ou efeitos apenas por serem comuns em sites de doceria. A referência visual real deve orientar as decisões.

## Estrutura sugerida da página

### 1. Cabeçalho

- Logotipo original.
- Navegação principal.
- Links para produtos, galeria e contato.
- Chamada para encomenda, se houver canal confirmado.
- Menu móvel acessível.

### 2. Hero

- Fotografia original em destaque.
- Nome oficial da marca.
- Copy original disponível.
- Chamada para ação funcional, se aplicável.

### 3. Produtos

- Produtos identificados nas publicações.
- Fotos originais.
- Nomes e descrições publicados.
- Preços apenas quando confirmados.
- Link para solicitar informações ou encomendar.

### 4. Galeria do Instagram

- Fotografias originais autorizadas.
- Layout responsivo e consistente.
- Links para publicações originais, quando disponíveis.
- Não simular um feed atualizado automaticamente sem integração real.

### 5. Sobre a marca

Utilizar somente a história, os valores e as informações institucionais confirmadas. Se não houver conteúdo suficiente, manter a seção compacta ou aguardar material do proprietário.

### 6. Encomendas e contato

- Canais oficiais confirmados.
- Link para WhatsApp, se o número estiver disponível.
- Formulário opcional com nome, produto, quantidade, data pretendida e mensagem.
- Validação dos campos e feedback acessível.
- Mensagem pré-preenchida no WhatsApp, quando aplicável.

Abrir uma conversa ou preparar uma mensagem não significa que o pedido foi confirmado.

### 7. Rodapé

Incluir apenas informações disponíveis e verificadas, como Instagram, WhatsApp, endereço, horários e informações institucionais.

## Regras de conteúdo e copy

- Preservar exatamente os textos originais da marca quando forem utilizados.
- Não reescrever, resumir ou corrigir a copy original.
- Não inventar slogans, depoimentos, avaliações ou promoções.
- Não inventar sabores, ingredientes, preços, prêmios ou disponibilidade.
- Criar textos funcionais de interface separadamente, quando necessário.
- Não apresentar conteúdo fictício como informação oficial.

## Responsividade e mobile-first

Breakpoints de referência:

- **Mobile:** abaixo de 768 px.
- **Tablet:** de 768 px a 1023 px.
- **Desktop:** a partir de 1024 px.

Requisitos:

- Começar pelo layout mobile.
- Evitar rolagem horizontal indevida.
- Manter textos legíveis sem zoom.
- Empilhar elementos quando necessário.
- Usar áreas de toque de pelo menos 44 × 44 px.
- Adaptar grids e imagens a cada tamanho de tela.
- Preservar a hierarquia visual em todos os dispositivos.

## Acessibilidade

- Utilizar HTML semântico: `header`, `nav`, `main`, `section`, `article` e `footer`.
- Manter uma hierarquia de títulos coerente.
- Adicionar textos alternativos descritivos às imagens.
- Associar `label` aos campos dos formulários.
- Garantir navegação por teclado.
- Exibir estados de foco claramente.
- Buscar conformidade com WCAG 2.2 nível AA, quando aplicável.
- Respeitar `prefers-reduced-motion`.
- Não comunicar informações apenas por cores.

## Performance

- Utilizar imagens responsivas com `srcset` e `sizes` quando possível.
- Preferir WebP ou AVIF quando disponíveis.
- Definir dimensões para reduzir mudanças de layout.
- Utilizar `loading="lazy"` nas imagens fora da primeira dobra.
- Priorizar corretamente a imagem principal.
- Evitar dependências e scripts desnecessários.
- Evitar vídeos automáticos pesados e animações excessivas.
- Utilizar URLs estáveis e autorizadas para as imagens.

## Interações

Implementar interações discretas e funcionais:

- Estados hover, focus e active.
- Navegação móvel acessível.
- Rolagem suave, quando apropriada.
- Feedback de validação dos formulários.
- Transições sutis alinhadas ao Design System.
- Respeito à preferência por movimento reduzido.

Não criar botões decorativos sem funcionalidade.

## Tecnologia e organização

Utilizar a stack já adotada pelo projeto. Para uma aplicação React, recomenda-se React, TypeScript e CSS organizado por componentes ou módulos.

Estrutura sugerida:

```text
src/
  components/
    Header
    Hero
    ProductGallery
    InstagramGallery
    ContactSection
    Footer
  sections/
  data/
    products
    gallery
    brand
  styles/
    tokens
    global
  assets/
    images
    logo
```

Adaptar a estrutura à tecnologia escolhida. Manter produtos, imagens, textos e links em estruturas fáceis de editar.

Não criar backend, banco de dados ou autenticação sem necessidade real. Planejar futuras evoluções, como catálogo gerenciável e painel administrativo, sem adicionar complexidade prematura.

## SEO e compartilhamento

- Definir título e descrição com informações verdadeiras e aprovadas.
- Configurar Open Graph para compartilhamento.
- Adicionar favicon baseado na identidade oficial, quando disponível.
- Utilizar URLs compreensíveis.
- Configurar URL canônica quando houver domínio definitivo.
- Incluir dados estruturados somente com informações verificadas.

Não inventar endereço, avaliações, preços ou horários em metadados ou dados estruturados.

## Tratamento das imagens

Preservar a aparência real dos produtos. Não alterar artificialmente cores, recheios, texturas, formatos, decorações ou embalagens. Ajustar `object-fit` e `object-position` conforme cada fotografia, evitando cortes que escondam detalhes importantes.

Utilizar arquivos originais em alta resolução e com autorização de uso no site.

## Plano de execução

1. Inspecionar as referências e os materiais disponíveis.
2. Extrair a identidade visual e definir os tokens.
3. Organizar fotos, legendas, produtos e links.
4. Definir a arquitetura da página e a hierarquia visual.
5. Implementar o layout responsivo mobile-first.
6. Implementar as interações e os canais de contato.
7. Verificar acessibilidade, SEO e performance.
8. Testar em diferentes resoluções e corrigir problemas.
9. Documentar os dados que ainda precisam ser fornecidos pelo proprietário.

## Checklist de aceite

- [ ] A identidade visual corresponde às referências disponíveis.
- [ ] As fotografias são da marca ou têm autorização de uso.
- [ ] A copy original foi preservada.
- [ ] Não existem produtos, preços ou depoimentos inventados.
- [ ] Todos os links foram testados.
- [ ] O contato abre o canal correto.
- [ ] O layout funciona em mobile, tablet e desktop.
- [ ] Não há rolagem horizontal indevida.
- [ ] Menu e formulários são acessíveis por teclado.
- [ ] As imagens possuem textos alternativos adequados.
- [ ] Contraste e foco são acessíveis.
- [ ] As imagens carregam de forma eficiente.
- [ ] Não há erros conhecidos no console ou links quebrados.
- [ ] Os componentes mantêm consistência visual.
- [ ] O site não parece um template genérico.

## Resultado esperado

Um website funcional, profissional e consistente com a identidade da **E de Chocolate Doceria**, que valorize as fotografias originais, apresente os produtos de maneira atraente e facilite o contato com os clientes.

A fidelidade às referências e à copy original tem prioridade sobre tendências visuais genéricas.

## Informações que podem ser necessárias

Para concluir o site com fidelidade, confirmar ou fornecer:

- Logotipo em boa resolução.
- Fotografias originais dos produtos.
- Capturas de tela do Instagram, caso o perfil não possa ser acessado.
- Legendas e textos que devem aparecer no site.
- Número oficial de WhatsApp ou outro canal de pedidos.
- Preços e informações de produtos, se forem exibidos.
- Endereço e horários, caso devam aparecer.
- Domínio e hospedagem, quando definidos.
