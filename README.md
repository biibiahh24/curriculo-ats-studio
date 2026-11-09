# CV Claro — gerador de currículo ATS

MVP educacional para organizar informações profissionais em uma estrutura simples, legível por pessoas e por sistemas de triagem de currículos.

- **Repositório:** https://github.com/biibiahh24/curriculo-ats-studio
- **Aplicação:** https://biibiahh24.github.io/curriculo-ats-studio/
- **Protótipo:** `index.html`

## Problema e público

Quem está procurando estágio ou emprego pode perder tempo ajustando o currículo para cada vaga e usar colunas, gráficos ou elementos que atrapalham a extração automática. O CV Claro oferece uma página única com campos convencionais, prévia em texto, checklist de estrutura, download .txt e impressão/Salvar como PDF.

## Tese do MVP

Se a pessoa conseguir conferir em poucos minutos se incluiu nome, contato, resumo, experiência, formação e competências, terá um currículo mais fácil de revisar e adaptar para a vaga. O MVP não pontua compatibilidade real com ATS nem garante aprovação.

**Métrica de validação:** testar com 5 estudantes; observar se conseguem preencher e exportar um currículo sem ajuda e perguntar se a checklist foi útil.

## Prompt de construção

> Crie um editor de currículo responsivo em português chamado CV Claro. Inclua campos para nome, contato e links, resumo profissional, experiências, formação e competências. Mostre uma prévia limpa com títulos convencionais, atualizada enquanto a pessoa escreve. Acrescente checklist de campos preenchidos, exportação de texto simples e impressão para PDF. Não use tabelas, colunas, gráficos, imagens, ícones no currículo ou pontuação inventada de ATS. Não invente fatos profissionais; use placeholders claros. Mantenha todos os dados apenas na página aberta e avise que o produto não garante aprovação em sistemas de triagem. Garanta rótulos acessíveis, teclado e layout adaptável a celular.

## Decisões e limites

- A estrutura prioriza texto simples e seções convencionais.
- A checklist conta campos preenchidos, não mede qualidade nem compatibilidade com um ATS específico.
- Os dados não são salvos em servidor; ao fechar a página, o conteúdo desaparece.
- O usuário deve adaptar palavras-chave à vaga sem incluir habilidades que não possui.
- O MVP não inclui login, upload de currículo existente ou geração automática com IA.

## Reflexão

Um gerador pode ajudar a organizar informações, mas não deve inventar experiência nem prometer que um currículo passará por qualquer filtro. A prévia e a exportação são simples de usar; testes com estudantes e leitura de arquivos exportados por diferentes sistemas são os próximos passos para validar a hipótese.

## Executar

Abra `index.html` em um navegador moderno. Para salvar em PDF, use **Imprimir / salvar PDF**.
