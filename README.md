# Sistema de Realidade Virtual para Treinamento de Segurança em Canteiro de Obras

Proposta de qualificação de mestrado apresentada ao **Programa de Pós-Graduação em Ciência da Computação da Universidade Federal do Ceará (UFC)**.

**Autor:** Abner Augusto Ramos Macedo Antunes de Souza
**Orientador:** Prof. Dr. Joaquim Bento
**Tipo:** Qualificação de Mestrado

---

## Sobre a pesquisa

Esta proposta apresenta o desenvolvimento de um **sistema de Realidade Virtual (RV)** para treinamento de segurança no trabalho em canteiros de obras, com foco na redução de acidentes por meio de uma abordagem imersiva.

O sistema simula cenários de risco conforme a **NR-18** (Norma Regulamentadora de Segurança e Saúde no Trabalho na Indústria da Construção), permitindo que trabalhadores pratiquem procedimentos de segurança em ambiente virtual antes de enfrentá-los no mundo real.

### Cenários simulados

- Seleção e uso de EPIs (Equipamentos de Proteção Individual)
- Trabalho em altura
- Movimentação de cargas

### Stack tecnológica

| Componente | Tecnologia |
|-----------|-----------|
| Motor gráfico | Unity 3D (C#) |
| SDK de RV | Meta XR SDK |
| Hardware alvo | Meta Quest 3 |

---

## Estrutura do repositório

```
proposta-qualificacao.tex        ← arquivo raiz LaTeX
lib/
  preambulo.tex                  ← pacotes e configurações
  ufctex.sty                     ← estilo UFC (não editar)
1-pre-textuais/                  ← resumo, siglas
2-textuais/                      ← capítulos (introdução → considerações finais)
3-pos-textuais/
  referencias.bib                ← referências BibTeX
  anexos/                        ← roteiro da experiência VR
```

---

## Como compilar

Requer **TeX Live 2026** (ou similar) com `latexmk` e `makeglossaries`.

```bash
latexmk -pdf -interaction=nonstopmode proposta-qualificacao.tex
makeglossaries proposta-qualificacao
latexmk -pdf -interaction=nonstopmode proposta-qualificacao.tex
```

No VS Code com a extensão LaTeX Workshop, o build dispara automaticamente ao salvar.

---

## Template base

Este documento usa o **ufctex** — template LaTeX adaptado do [abnTeX2](https://github.com/abntex/abntex2) para a Universidade Federal do Ceará, com formatação conforme as normas ABNT.

O README original do template está em [README-template.md](README-template.md).

---

## Licença

Documento acadêmico de uso restrito ao processo de qualificação de mestrado da UFC.
