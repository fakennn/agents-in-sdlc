---
title: "Lição 12 - Implante o site no GitHub Pages"
description: "Use o aplicativo GitHub Copilot para configurar um workflow do Pages, revisar o pull request e verificar o Space Quiz publicado."
authors:
  - jamesmontemagno
lastUpdated: 2026-10-12
---

Publique o Space Quiz no GitHub Pages para que todos possam acessá-lo. O Copilot pode preparar o workflow e orientar a implantação, mas você continua responsável por revisar as mudanças e confirmar que o site está disponível.

Nesta lição, você vai:

- pedir ao Copilot para configurar a implantação no GitHub Pages.
- revisar o workflow e o pull request antes de fazer o merge.
- acompanhar a implantação e verificar o site publicado.

## Cenário

O Space Quiz já está em um repositório do GitHub, mas as pessoas ainda precisam de uma forma simples de experimentá-lo. Publicar o site de arquivo único com o GitHub Pages o disponibiliza em uma URL pública, sem adicionar servidor ou dependência de runtime.

## Peça ao Copilot para implantar o site

Na sessão do aplicativo Copilot para `space-quiz`, envie este prompt:

```plaintext
Enable GitHub Pages for this repository. Create a GitHub Actions workflow that builds the website if needed and deploys it to GitHub Pages. Add a README describing the app and how to run it locally if one does not already exist. Create a pull request with these changes and merge it after required checks pass. Monitor the deployment until it succeeds, then report the final URL of the live website. If you lack permission to enable Pages or merge, tell me exactly what I need to approve or do; do not report success until the site is live.
```

![Diagrama em três etapas: um pull request do space-quiz mesclado; uma execução bem-sucedida de Deploy website no GitHub Actions com as etapas Build website, Upload artifact e Deploy to Pages; e o Space Quiz publicado em yourname.github.io/space-quiz/.](../../../_images/first-steps-app-pages-deploy.svg)

> [!WARNING]
> Este prompt pede que o agente crie e faça merge de um pull request e altere as configurações de Pages do repositório. Revise as diferenças, as permissões de implantação e quaisquer solicitações de aprovação do GitHub antes de continuar.

## Revise o workflow e verifique a implantação

1. Confirme que o README só foi adicionado se o repositório ainda não tinha um.
2. Revise as mudanças do pull request, incluindo as etapas de build e implantação do workflow.
3. Faça o merge somente depois que as verificações obrigatórias do pull request forem aprovadas.
4. Acompanhe a execução de implantação do GitHub Actions até ela ser concluída com sucesso.
5. Abra a URL informada e confirme que o Space Quiz carrega.

Se o agente não puder habilitar o Pages ou fazer merge do pull request, siga as instruções específicas que ele fornecer. Só considere a tarefa concluída depois que a implantação tiver sucesso e o site publicado carregar.

## Resumo e próximas etapas

O Space Quiz está disponível como um site publicado, e você verificou a implantação em vez de confiar apenas no relatório do agente. Continue para a [lição 13: Revisão e próximas etapas][next-lesson].

[next-lesson]: ../13-review/
