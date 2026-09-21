# Formulários Mari

Repositório central pros formulários de qualificação da Mariana Manfredinny. Cada formulário vive na sua própria pasta, com o mesmo sistema visual (liquid glass / janela macOS / status bar iOS no mobile), mudando só a copy e a lógica de qualificação.

## Estrutura

```
/nome-do-formulario
  index.html      → página completa (HTML + CSS + JS inline, sem build)
  <foto>.jpg       → imagem de fundo
```

## Formulários

- `intensivo-1x1/` — formulário de qualificação pro Intensivo 1X1 (sessão individual, R$1.000).

## Como funciona um formulário novo

1. Copiar a estrutura de um formulário existente como base.
2. Trocar perguntas, opções e textos de tela conforme a copy enviada.
3. Cada pergunta desqualificante leva a uma tela de trava própria (nunca genérica demais, nunca desmerecendo o lead).
4. Ajustar o `ENDPOINT` do Formspree e o evento do `dataLayer` (GTM) no final do `<script>`.
5. Publicar a pasta como subdomínio (CNAME) ou hospedar via GitHub Pages.

## GTM

O GTM (`GTM-WJ99QGK8`) é o mesmo container usado em todos os sites da Mari — instalado uma vez, tags e pixels novos são configurados direto no GTM em vez de mexer em cada página.
