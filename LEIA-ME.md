# Bio da Ketlin — clone do Beacons (tema preto)

Clone de `beacons.ai/ketlin.lemos` com fundo preto no lugar do rosa.

## Arte
`assets/hero.jpg` — a arte "Ketlin Lemos" (1024x1536, proporção 2:3).
Para trocar, substitua o arquivo mantendo o mesmo nome. Se a proporção mudar,
ajuste o `aspect-ratio` no CSS do `.hero img`.

## O que tem na página
- Arte no topo, ocupando a largura toda, dissolvendo no preto
- **Sem** o texto "Ketlin Lemos" que o Beacons mostrava (a arte já traz o nome)
- Legenda logo abaixo da foto: "Confira todas as casas que eu jogo 🚀"
- Ícone do Instagram (@ketlin.bet)
- Os 5 links, **exatamente as mesmas URLs do Beacons**, na mesma ordem
- Pop-up +18 antes de entrar nas casas — o nome da casa muda conforme o link
- Rodapé com selo de SSL + aviso legal de jogo responsável

## Os links (conferidos 1 a 1 contra o Beacons)
1. LOTTU BET — `lottu.bet.br/register?...ngx_source_id=ket&utm_campaign=ket`
2. ONABET — `onabet.cxclick.com/visit/?bta=122126&brand=onabet&utm_campaign=ket`
3. ESPORTES DA SORTE — `go.aff.esportesdasorte.bet.br/nan5y1w7?campaign_id=28849&utm_campaign=ket`
4. NOVIBET — `rt.novibet.partners/o/AKaX3F?site_id=1022923`
5. CANAL NO TELEGRAM — `t.me/addlist/CvcgyjK97_c2NDgx`

Instagram: `instagram.com/ketlin.bet`

## Mexer nos links
Tudo fica no array `LINKS` dentro do `index.html` (perto do fim).
- `gate:true`  → mostra o pop-up +18
- `casa:"..."` → nome que aparece no pop-up ("Você está indo para ...")
- `gate:false` → abre direto (Telegram)

## Pop-up: quantas vezes pergunta
Pergunta 1x por visita (guarda no `sessionStorage`).
Para perguntar sempre, apague a linha `marcarConfirmado();` no `ovYes`.

## Selo SSL
O selo verde só acende quando o site está publicado em HTTPS.
Rodando local ele mostra "PRÉ-VISUALIZAÇÃO LOCAL" — é o comportamento certo.

## Publicar
Mesmo esquema dos outros: sobe a pasta no GitHub Pages e aponta o domínio
(criar o `CNAME` com o domínio quando for definir qual será).
