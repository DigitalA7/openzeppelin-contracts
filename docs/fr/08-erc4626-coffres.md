# ERC-4626 : parts de coffre

Un coffre reçoit un actif ERC-20 et émet des parts ERC-20.
`deposit` fixe les actifs déposés ; `mint` fixe les parts reçues ; `withdraw` fixe les actifs retirés ; `redeem` fixe les parts brûlées.
Les fonctions `preview*` estiment le résultat ; `max*` décrivent les limites. Une estimation ne réserve pas le taux futur.
**Exemple simplifié :** 120 actifs pour 100 parts correspondent à environ 1,2 actif par part. Le calcul exact inclut ici des arrondis et des actifs/parts virtuels.
**Piège :** le standard ne promet aucun rendement. Frais, pertes et dépôts directs modifient les résultats ; la base ne fournit pas de stratégie de placement.

[Code](../../contracts/token/ERC20/extensions/ERC4626.sol) · [Tests](../../test/token/ERC20/extensions/ERC4626.test.js) · [Arrondis](../modules/ROOT/pages/erc4626.adoc)

[Suite : Permit et transferts signes](09-permit-et-signatures.md)
