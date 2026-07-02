# WSRTA — pacote de atualização (assinado)

Este repositório guarda **somente o último** pacote de atualização do WSRTA:
`wsrta-update.zip` + `wsrta-update.zip.sig` (assinatura ed25519 dos bytes do zip). O painel
(botão *Atualizar painel* / ação `panel_update`) baixa ambos e o daemon **verifica a assinatura
com a chave pública embarcada ANTES de extrair/executar** — um repo comprometido não vira RCE
root. Cada release substitui o anterior (sem histórico, por design).
