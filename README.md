# Diagnóstico TI Page

Página estática do diagnóstico de conhecimentos em informática para entrevista/vaga administrativa.

## Hospedagem recomendada

Cloudflare Pages.

## Arquivo principal

- `index.html`

## Configuração importante

No `index.html`, procure:

```js
const LEAD = {
  ativo: true,
  endpoint: "https://SEU_APP_RAILWAY.up.railway.app/lead",
  permitir_pular: true
};
```

Depois que publicar a API no Railway, substitua `https://SEU_APP_RAILWAY.up.railway.app/lead` pela URL real da sua API.

Exemplo:

```js
endpoint: "https://diagnostico-ti-api-production.up.railway.app/lead"
```

## Fluxo

Instagram/Reels/Stories → Cloudflare Pages → API Railway → e-mail do seguidor + lead salvo.
