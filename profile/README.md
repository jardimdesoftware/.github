# 🌳 Jardim de Software

[![Followers](https://img.shields.io/github/followers/jardimdesoftware?label=Followers\&style=social)](https://github.com/jardimdesoftware)
[![Org stars](https://img.shields.io/github/stars/jardimdesoftware?label=Org%20Stars)](https://github.com/jardimdesoftware)
[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Website](https://img.shields.io/website?url=https%3A%2F%2Fuol.com.br\&label=website)](https://portal.ifpe.edu.br/)

> Repositório central da "fábrica" de software — templates, projetos didáticos, infra e material de apoio para desenvolvimento, infraestrutura e automação.

---

## Índice

1. [Sobre](#sobre)
2. [Objetivos](#objetivos)
3. [O que você encontra aqui](#o-que-voce-encontra-aqui)
4. [Como os projetos estão organizados](#como-os-projetos-estao-organizados)
5. [Contribuindo](#contribuindo)
6. [Onboarding / Mantainers](#onboarding--mantainers)
7. [Licença e Código de Conduta](#licenca-e-codigo-de-conduta)
8. [Templates & Automatizações](#templates--automatizacoes)
9. [CI/CD e Runners self-hosted](#cicd-e-runners-self-hosted)
10. [Como solicitar um novo projeto](#como-solicitar-um-novo-projeto)
11. [Contato / Comunidade](#contato--comunidade)

---

## Sobre

O Jardim de Software é a organização que centraliza os repositórios criados pela fábrica: desde *boilerplates* e templates (front, back, infra), projetos educativos e comerciais, experimentos de infra (Proxmox, Kubernetes, Rancher) e integrações de CI/CD. Nosso foco é educação prática, automação e reutilização.

## Objetivos

* Facilitar o aprendizado prático em desenvolvimento e infraestrutura.
* Fornecer templates reutilizáveis e padrões para acelerar o início de novos projetos.
* Promover boas práticas de Git, CI/CD, infraestrutura como código e DevSecOps.

## O que voce encontra aqui

* **Templates**: front-end (Next.js), back-end (.NET/Spring/Node), infra (Terraform/Ansible), Dockerfiles etc.
* **Projetos didáticos**: exercícios, exemplos de disciplinas e material para estudantes.
* **Infra**: exemplos de configuração Proxmox, runners self-hosted, scripts de automação.
* **Ferramentas da fábrica**: GitHub Actions, templates de issue/PR, geradores de repositório.

## Como os projetos estao organizados

Padrões sugeridos para repositórios nesta organização:

* `template-<tipo>-<nome>` — ex: `template-front-nextjs`, `template-back-spring`.
* `proj-<nome>-<ano>` — projetos disciplinares ou entregas de turma.
* `infra-<componente>` — scripts, playbooks e IaC (ex: `infra-proxmox`, `infra-runners`).

Branches principais:

* `main` — versão pronta para uso/produção.
* `develop` — desenvolvimento integrado (opcional para templates).
* `feature/<nome>` — para desenvolvimento de features.

Tags: **semântica** sugerida `vMAJOR.MINOR.PATCH` para releases.

## Contribuindo

Quer contribuir? Obrigado — você é bem-vindo! Siga este fluxo:

1. Abra uma **issue** descrevendo a sugestão ou bug.
2. Discuta a proposta (se necessário) e aguarde aprovação do maintainer.
3. Abra um **pull request** a partir de um branch `feature/ fix/` etc, com descrições claras e checklist.
4. Certifique-se de que o PR roda nos checks (linters, testes, build).

Arquivos úteis (colocar em `.github/` de cada repo):

* `CONTRIBUTING.md` (guia específico do repo)
* `ISSUE_TEMPLATE.md`
* `PULL_REQUEST_TEMPLATE.md`
* `CODE_OF_CONDUCT.md`

### Checklist rápido para PRs em templates

* [ ] README atualizado com exemplos de uso
* [ ] Dockerfile e/ou compose testados
* [ ] CI mínima (build e lint) configurada
* [ ] Licença/atribuições corretas

## Onboarding / Mantainers

Se você quer ser maintainer de um repositório da organização, abra uma issue com:

* Nome GitHub
* Repositório(s) que quer manter
* Experiência / motivação curta

Perfis de cargo sugeridos dentro da organização:

* *Owner* — administradores da organização (poucos).
* *Maintainer* — responsáveis por um ou mais repositórios.
* *Contributor* — contribuições avulsas.

## Licenca e Codigo de Conduta

Adotamos **Apache-2.0** para os projetos da organização. Cada repositório deve conter um `LICENSE` e um `CODE_OF_CONDUCT.md`.

> Se você preferir outra licença (MIT, GPLv3), adicione a justificação no repo antes de publicar.

## Templates & Automatizacoes

Temos templates para:

* Frontend (Next.js) — `template-front-nextjs`
* Backend (Java Spring / Node) — `template-back-<stack>`
* Infra (Terraform + Ansible) — `template-infra-<cloud/onprem>`
* GitHub Actions: lint, build, publish container, scanner de segurança

Também temos o repo `infra-factory` com os scripts/Actions que geram repositórios novos automaticamente.

## CI/CD e Runners self-hosted

Se o repositório criado usar runners self-hosted, documente no repo `infra-runners`:

* Como registrar um runner
* Labels usados (ex: `linux,gpu,proxmox`)
* Regras de segurança e acesso

Para Actions, inclua checks mínimos: `lint`, `build`, `container-scan`.

## Como solicitar um novo projeto

Crie uma **issue** no repositório `infra-factory` (desta de organização) preenchendo o template com:

* Título: `<nome do projeto>`
* Nome do sistema: `<nome do sistema>`
* Template escolhido.
* Local de deployment.
* Credenciais necessárias para deployment.

Um maintainer revisará e o repositório será criado quando aprovado.

## Contato / Comunidade

* E-mail: `jardimdesoftware@belojardim.ifpe.edu.br`
* Issues: abra issues nos repositórios correspondentes

---




