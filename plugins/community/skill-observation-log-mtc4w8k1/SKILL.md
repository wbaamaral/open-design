# Skill Observation Log

Observations captured during task-oriented work.

**Status key:** OPEN = not yet actioned | ACTIONED (YYYY-MM-DD) = skill updated/created | DECLINED (YYYY-MM-DD) = user decided not to pursue — resolved statuses always carry their resolution date

---

## 2026-08-27

### Observation 1: Identidade Git precisa ficar fora da política versionada

**Status:** OPEN
**Date:** 2026-08-27
**Session context:** Levantamento de padrões de especificação, Git e qualidade para um projeto web.
**Skill:** New skill candidate: governança Git multi-colaborador
**Type:** open-source
**Phase/Area:** Workflow Git e segurança

**Issue:** Documentos e templates de processo podem fixar nome e e-mail de uma pessoa no repositório, o que dificulta colaboração e expõe dados que não precisam ser versionados.

**Suggested improvement:** Definir perfis de identidade em configuração local do usuário, com pré-voo que valida a identidade selecionada e altera a configuração local somente por ação explícita.

**Principle:** Políticas versionadas devem validar identidade humana sem armazenar identificadores pessoais; dados de identidade pertencem à configuração local e consentida de cada colaborador.

### Observation 2: Canonicalização deve preservar caminhos de referência ativos

**Status:** OPEN
**Date:** 2026-08-27
**Session context:** Formalização de uma especificação técnica aprovada em uma nova árvore normativa.
**Skill:** New skill candidate: migração documental segura
**Type:** open-source
**Phase/Area:** Documentação e rastreabilidade

**Issue:** Mover um documento aprovado para uma fonte canônica pode quebrar abas abertas, links
internos e referências históricas, mesmo quando o conteúdo foi preservado.

**Suggested improvement:** Ao canonizar documentação, migrar o conteúdo para a fonte normativa e
deixar no caminho anterior um redirecionamento curto que explique a mudança e aponte para a
referência canônica; em seguida validar os links locais.

**Principle:** Uma mudança de governança documental precisa preservar a navegabilidade do
histórico e tornar explícito qual arquivo recebe alterações normativas futuras.

### Observation 3: Renomeação de diretório exige validação estrutural

**Status:** OPEN
**Date:** 2026-08-27
**Session context:** Correção de referências após a substituição do diretório redundante por
`spec/especificacoes/`.
**Skill:** New skill candidate: migração documental segura
**Type:** open-source
**Phase/Area:** Documentação e rastreabilidade

**Issue:** A mudança de nomenclatura pode atualizar somente parte dos links e manter o diretório
antigo ou referências relativas nos documentos associados.

**Suggested improvement:** Tratar a mudança como uma operação única: mover os arquivos,
atualizar links e árvores de navegação, buscar o caminho anterior no repositório e validar cada
link local.

**Principle:** A migração de uma estrutura documental termina quando o caminho antigo deixa de
existir, os links apontam ao destino canônico e a navegação local continua resolvendo.

<!-- Checkpoint de acompanhamento (2026-08-27): nenhuma observação adicional após três itens
reconciliados. -->

### Observation 4: Paridade de marca deve usar papéis visuais

**Status:** OPEN
**Date:** 2026-08-27
**Session context:** Planejamento de identidade visual para aplicações digitais e impressas.
**Skill:** New skill candidate: sistema de marca multimeio
**Type:** open-source
**Phase/Area:** Estratégia de marca e produção

**Issue:** Repetir valores RGB em impressão ignora perfil de cor, papel e processo de produção,
o que quebra a consistência que a marca tenta preservar entre meios.

**Suggested improvement:** Definir tokens por papel visual e registrar conversões de impressão
somente depois de uma prova aprovada com o perfil ICC da gráfica.

**Principle:** Uma marca mantém paridade entre meios quando preserva hierarquia, contraste e
função das cores, não quando copia valores numéricos entre espaços de cor diferentes.

### Observation 5: Separar regras de marca de dados de contato

**Status:** OPEN
**Date:** 2026-08-27
**Session context:** Produção de um kit de identidade visual com cartão e guia de aplicações.
**Skill:** New skill candidate: sistema de marca multimeio
**Type:** open-source
**Phase/Area:** Arquitetura de arquivos de marca

**Issue:** Um modelo concreto de papelaria precisa de dados reais para mostrar hierarquia e
densidade, mas colocar esses dados na especificação canônica reduz sua reutilização e aumenta a
superfície de dados pessoais versionados.

**Suggested improvement:** Manter tokens, logotipos e regras em arquivos canônicos sem dados
pessoais; aplicar nome, contatos e endereço apenas nos modelos de peça que realmente os exigem.

**Principle:** Um sistema de marca fica reutilizável quando separa elementos estáveis da
identidade visual dos dados variáveis de cada aplicação.

### Observation 6: Restrições de impressão precisam de orçamento de layout

**Status:** OPEN
**Date:** 2026-08-27
**Session context:** Reconciliação entre uma especificação de marca e um modelo de cartão.
**Skill:** New skill candidate: sistema de marca multimeio
**Type:** open-source
**Phase/Area:** Pré-impressão e verificação

**Issue:** Elevar o tamanho mínimo de texto depois de compor uma peça impressa pode provocar
estouro de conteúdo, mesmo quando a grade, a sangria e a área segura parecem corretas.

**Suggested improvement:** Antes de fechar um modelo físico, calcular o orçamento da área segura
com tamanho mínimo, entrelinha, linhas de conteúdo e escala do logotipo; ajustar as quebras de
texto antes da exportação.

**Principle:** Formato físico, área segura e legibilidade definem a composição antes de qualquer
ajuste estético de escala ou espaçamento.

### Observation 7: Sistema de ícones deve escolher o meio antes da ferramenta

**Status:** OPEN
**Date:** 2026-08-27
**Session context:** Revisão de ícones funcionais em um cartão de visita impresso.
**Skill:** Existing skill: imagegen
**Type:** open-source
**Phase/Area:** Decisão de formato de ativo

**Issue:** Um pedido de melhoria visual pode chegar por um fluxo de imagem mesmo quando o ativo
precisa permanecer vetorial para manter traço, escala e nitidez no material impresso.

**Suggested improvement:** Incluir uma verificação explícita de meio e escalabilidade antes de
gerar qualquer imagem; para ícones, marcas e elementos de impressão, encaminhar a edição para
SVG ou código nativo quando isso preservar melhor os requisitos.

**Principle:** O meio de uso define a tecnologia do ativo; raster só entra quando aumenta a
fidelidade da entrega final.

## Provenance

Formalized by OpenDesign from candidate cf8ff037-fef0-4b28-9184-32b9f9e65ce3.
