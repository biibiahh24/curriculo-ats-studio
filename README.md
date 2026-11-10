# CV Claro — comparação de currículo com vaga

Aplicação educacional para comparar uma descrição de vaga com um currículo, mostrar termos presentes e ausentes e organizar uma cópia simples para revisão. O projeto prioriza legibilidade por ATS e transparência: não inventa qualificações e não promete aprovação.

- **Aplicação publicada:** https://biibiahh24.github.io/curriculo-ats-studio/
- **Repositório:** https://github.com/biibiahh24/curriculo-ats-studio
- **Tecnologias:** HTML, CSS e JavaScript puro; sem dependências ou chaves de API.
- **Arquivo principal:** `index.html`

## Problema que resolve

Quem procura uma oportunidade precisa adaptar o currículo à vaga sem perder tempo com formatações que atrapalham a leitura automática. O CV Claro compara os dois textos no próprio navegador, aponta termos que aparecem no currículo e termos que merecem revisão, e organiza o texto atual em uma versão simples para copiar, baixar ou imprimir.

## Prompt de especificação

> Crie uma aplicação web responsiva em português chamada CV Claro para comparar um currículo e uma descrição de vaga. A pessoa deve poder colar os dois textos. Compare termos relevantes da vaga com o currículo, apresente uma estimativa simples de correspondência, liste os termos encontrados e os que não foram localizados, e organize uma versão do currículo para revisão, com opções de copiar, baixar em TXT e imprimir/salvar em PDF. Use um visual claro, acessível, responsivo e com hierarquia tipográfica. Não invente experiência, formação, resultados ou competências. Não inclua automaticamente termos ausentes: mostre-os apenas como sugestões para a pessoa conferir. Avise que a pontuação é uma estimativa do protótipo, não a nota de um ATS real. Mantenha os textos localmente na página, sem servidor, login, analytics ou chamadas externas. Use títulos convencionais e conteúdo em texto simples.

## Como a análise funciona

1. A pessoa cola a descrição da oportunidade e seu currículo.
2. O protótipo normaliza maiúsculas e acentos e extrai termos de pelo menos três caracteres, removendo palavras muito comuns.
3. A lista prioriza os termos mais repetidos na vaga e compara sua presença no currículo.
4. A estimativa é a proporção de termos considerados que aparecem no texto. O resultado também separa termos encontrados e não localizados.
5. A versão para revisão preserva o currículo colado e acrescenta somente uma lista de termos que já estavam presentes no texto. Os termos ausentes não são inseridos.
6. A pessoa revisa tudo antes de copiar, baixar como TXT ou imprimir/salvar em PDF.

## Evolução e ajustes

A primeira versão era um editor de currículo com campos separados, prévia e checklist de preenchimento. Ao comparar essa ideia com o desafio, ficou claro que ela não atendia ao fluxo principal pedido: analisar uma vaga junto com o currículo.

A versão final foi reorganizada para receber os dois textos e mostrar a comparação antes de gerar a cópia para revisão. Também foram acrescentados exportação, impressão, limpeza dos campos e avisos explícitos sobre privacidade e limites da pontuação. A saída mantém o conteúdo original para evitar alterações ou fatos inventados.

## Decisões e limites

- A comparação é textual e não reproduz os critérios de um sistema ATS comercial.
- Termos podem ter sinônimos, variações de escrita ou significados diferentes que a análise simples não reconhece.
- A pontuação não prevê entrevista, classificação ou contratação.
- Os dados não são enviados a um servidor e desaparecem quando a página é fechada.
- Termos ausentes devem ser incluídos somente se corresponderem à experiência real da pessoa.
- O projeto não oferece upload de arquivo, login, armazenamento, integração com IA ou garantia de aprovação.

## Como usar localmente

Abra `index.html` em um navegador moderno. Não é necessário instalar dependências. Na aplicação publicada, cole os textos, clique em **Analisar compatibilidade** e revise a saída antes de usar.

## Próximos passos possíveis

- reconhecer sinônimos e expressões compostas em português;
- permitir importar DOCX/PDF com consentimento e processamento local;
- adicionar testes com pessoas candidatas e comparar a extração em diferentes ATS;
- oferecer exportação DOCX preservando a ordem de leitura.
