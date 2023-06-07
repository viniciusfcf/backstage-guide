# [Backstage](https://backstage.io)

# backstage-guide

# O que é backstage?
Plataforma para construir portais para os desenvolvedores, arquitetos...

# Glossário
componente = serviços, biblioteca, APIS, pipelines, funcionalidades mobile, websites internos...


# O que resolve
- Empresas que têm diversos times e implantam diversos sistemas/serviços normalmente enfrentam problemas na padronização de frameworks, versões, modelo de implantação, configuração, observabilidade.
- Engenheiros normalmente criam e fazem implantação de componentes, sem um processo adequado têm uma baixa performance e baixo índice de reaproveitamento dos componentes gerados.
- Existe uma grande fragmentação de informação sobre os componentes existentes

# O paradoxo dos padrões
Ao centralizar serviços e padronizar suas ferramentas, o Backstage agiliza seu ambiente de desenvolvimento de ponta a ponta. Em vez de restringir a autonomia, a padronização libera seus engenheiros da complexidade da infraestrutura. Assim, você pode voltar a construir e dimensionar com rapidez e segurança.


# O que fazemos de fato no Backestage?
Criamos, gerenciamos e exploramos componentes

# O que não é
- Fonte de verdade (pense como se fosse um frontend para visualizar dados de todos os sistemas)

# Extensibilidade com [Plugins](https://backstage.io/docs/overview/architecture-overview#plugins-and-plugin-backends)
É possível extender o Backstage criando plugins. Eles são criados em TypeScript ou JavaScript

# Resumo
Pense no Backstage como o ponto inicial para procurar qualquer informação sobre componentes da sua empresa/time. Essas informações podem ser: documentação, versão atual, equipe responsável, estado do deploy, link para ver os logs, link para o Grafana, localização do código fonte.

Fonte: https://backstage.io/

# Como iniciar este backstage

## Prerequirements

https://backstage.spotify.com/learn/standing-up-backstage/

## Subir um banco de dados postgres
- https://backstage.io/docs/tutorials/configuring-plugin-databases
- https://backstage.io/docs/tutorials/switching-sqlite-postgres/

## Definir integração com github

- definir envs:(https://backstage.io/docs/getting-started/configuration#setting-up-a-github-integration)
  - GITHUB_BACKSTAGE_TOKEN=...
  - GITHUB_BACKSTAGE_CLIENTID=...
  - GITHUB_BACKSTAGE_SECRET=...

## Subir em modo dev

```sh
yarn install
yarn dev
```