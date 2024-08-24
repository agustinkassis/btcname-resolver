# btcname-resolver
BTC Name resolver

# Purpose
Provide a simple API that resolves btcname from ordinals. Following this standard
https://docs.btcname.id/docs/overview/chapter-4-thinking-about-.btc-domain-name/name-routing

## Steps
- Resolve btc domain name and get inscriptionID
- Request $ordserver/inscription/{INSCRIPTIONID}i0 and get satpoint
- Request $ordserver/output/${satpoint} <-- remove the last :0
