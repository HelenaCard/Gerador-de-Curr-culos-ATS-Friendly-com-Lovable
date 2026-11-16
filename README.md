# CV Match AI

## Sobre o projeto

O **CV Match AI** é uma aplicação web que utiliza inteligência
artificial para comparar um currículo com a descrição de uma vaga de
emprego. A plataforma identifica correspondências e possíveis lacunas,
apresenta sugestões de melhoria e auxilia o candidato a criar uma versão
mais clara e compatível com sistemas ATS (*Applicant Tracking Systems*).

A proposta é ajudar estudantes, recém-formados e profissionais em busca
de novas oportunidades a adaptar a apresentação de suas experiências e
competências aos requisitos de cada vaga --- sem inventar informações ou
qualificações.

## Objetivos

-   Facilitar a análise de compatibilidade entre currículos e vagas.
-   Identificar habilidades, experiências e palavras-chave relevantes.
-   Apontar requisitos atendidos, parcialmente atendidos e não
    identificados.
-   Oferecer recomendações práticas para melhorar o currículo.
-   Permitir editar e exportar uma versão otimizada do documento.

## Funcionalidades previstas

  -----------------------------------------------------------------------
  Funcionalidade                      Descrição
  ----------------------------------- -----------------------------------
  Envio de currículo                  Upload de arquivos PDF ou DOCX.

  Descrição da vaga                   Inserção de texto ou envio de
                                      arquivo com os requisitos da
                                      oportunidade.

  Análise inteligente                 Extração e interpretação das
                                      informações do currículo e da vaga.

  Comparação                          Identificação de correspondências e
                                      lacunas entre os documentos.

  Relatório                           Apresentação de compatibilidade
                                      estimada, pontos fortes e
                                      sugestões.

  Editor                              Revisão e edição das seções do
                                      currículo.

  Exportação                          Geração do currículo otimizado em
                                      PDF e, quando disponível, DOCX.

  Histórico                           Consulta de análises anteriores,
                                      conforme implementação.
  -----------------------------------------------------------------------

## Como funciona

1.  **Envio:** o usuário adiciona seu currículo e informa a descrição da
    vaga.
2.  **Extração:** o sistema identifica dados profissionais, formação,
    experiências, cursos e habilidades.
3.  **Interpretação:** a inteligência artificial organiza os requisitos
    obrigatórios e desejáveis da vaga.
4.  **Comparação:** o sistema verifica quais requisitos estão presentes,
    parcialmente presentes ou não foram identificados no currículo.
5.  **Diagnóstico:** é gerado um relatório com pontos fortes, lacunas e
    oportunidades de melhoria.
6.  **Otimização:** o usuário revisa as sugestões e edita o currículo.
7.  **Exportação:** a versão final pode ser baixada nos formatos
    disponibilizados pela aplicação.

## Tecnologias

A arquitetura planejada considera as seguintes tecnologias:

  Tecnologia     Utilização
  -------------- -------------------------------------------------------
  Lovable        Desenvolvimento assistido da aplicação.
  React          Construção da interface.
  Tailwind CSS   Estilização e responsividade.
  Supabase       Autenticação, banco de dados e armazenamento privado.
  API de IA      Extração, comparação e geração de sugestões.

> A disponibilidade de cada integração depende da configuração realizada
> no projeto. Ajuste esta lista conforme as tecnologias efetivamente
> utilizadas na implementação.

## Identidade visual

O CV Match AI utiliza uma identidade visual tecnológica, profissional e
minimalista.

  -----------------------------------------------------------------------
  Cor                     Código                  Aplicação
  ----------------------- ----------------------- -----------------------
  Azul-marinho            `#142B4A`               Identidade principal e
                                                  elementos de destaque.

  Azul elétrico           `#3478F6`               Botões, links e ações.

  Branco                  `#FFFFFF`               Cards e superfícies.

  Cinza claro             `#F4F7FB`               Fundos e áreas de
                                                  apoio.

  Verde                   `#16A078`               Indicadores positivos.

  Amarelo                 `#F2B84B`               Alertas e pontos de
                                                  atenção.
  -----------------------------------------------------------------------

**Tipografia:** Inter ou Manrope.

## Estrutura de telas

-   **Landing Page:** apresentação da plataforma, benefícios e acesso à
    análise.
-   **Dashboard:** visão geral e histórico das análises.
-   **Envio de documentos:** upload do currículo e inserção da vaga.
-   **Resultado:** relatório de compatibilidade e recomendações.
-   **Editor:** revisão e personalização do currículo otimizado.
-   **Exportação:** pré-visualização e download do documento.

## Regras e cuidados da análise

-   Não inventar experiências profissionais, cursos, habilidades ou
    qualificações.
-   Não alterar fatos ou informações pessoais do candidato.
-   Recomendar palavras-chave somente quando forem coerentes com a
    experiência real.
-   Explicar o motivo das sugestões sempre que possível.
-   Diferenciar requisitos atendidos, parcialmente atendidos e não
    identificados.
-   Tratar a pontuação como uma estimativa baseada nos critérios
    apresentados.

**Importante:** uma pontuação de compatibilidade não representa a chance
de contratação nem garante aprovação em um sistema ATS. Cada plataforma
de recrutamento pode utilizar critérios diferentes.

## Privacidade e segurança

Currículos podem conter dados pessoais. A implementação deve considerar
a Lei Geral de Proteção de Dados (LGPD), incluindo:

-   Armazenamento privado e controle de acesso aos documentos.
-   Proteção das informações e das credenciais de API.
-   Processamento de dados sensíveis à segurança no servidor, evitando
    expor chaves no navegador.
-   Validação dos arquivos enviados.
-   Política clara de retenção e exclusão de documentos.
-   Uso dos dados somente para finalidades informadas ao usuário.

## Como executar

As instruções abaixo são uma referência para quando o projeto estiver
disponível em um ambiente React.

1.  Clone o repositório:

    ``` bash
    git clone URL_DO_REPOSITORIO
    ```

2.  Acesse a pasta:

    ``` bash
    cd cv-match-ai
    ```

3.  Instale as dependências:

    ``` bash
    npm install
    ```

4.  Configure as variáveis de ambiente necessárias para as integrações.
    Consulte a documentação do projeto e utilize um arquivo `.env`
    local, sem publicar credenciais.

5.  Inicie o ambiente de desenvolvimento:

    ``` bash
    npm run dev
    ```

> Os comandos e variáveis podem variar conforme a estrutura gerada pelo
> Lovable. Confira o `package.json` e a configuração real do projeto
> antes de executar.

## Escopo do MVP

A primeira versão prioriza o fluxo principal:

-   [ ] Upload de currículo em PDF ou DOCX.
-   [ ] Inserção da descrição da vaga.
-   [ ] Extração das informações dos documentos.
-   [ ] Comparação entre currículo e vaga.
-   [ ] Relatório de compatibilidade.
-   [ ] Sugestões de otimização.
-   [ ] Edição do currículo.
-   [ ] Exportação do documento final.

Funcionalidades como histórico avançado, múltiplos modelos de currículo
e recursos adicionais podem ser incorporadas em versões futuras.

## Público-alvo

-   Estudantes em busca de estágio.
-   Pessoas em início de carreira.
-   Profissionais em transição de carreira.
-   Candidatos que desejam adaptar seus currículos a diferentes
    oportunidades.

## Contribuição

Sugestões, melhorias e identificação de problemas são bem-vindas. Para
contribuir:

1.  Faça um fork do repositório.
2.  Crie uma branch para sua alteração.
3.  Faça commits objetivos.
4.  Abra um Pull Request explicando as mudanças.

## Projeto: https://pixel-perfect-picture-6803.lovable.app/

## Licença
-----

------------------------------------------------------------------------

```{=html}
<p align="center">
```
Desenvolvido como projeto de aplicação de tecnologia e inteligência
artificial ao desenvolvimento profissional.
```{=html}
</p>
```
