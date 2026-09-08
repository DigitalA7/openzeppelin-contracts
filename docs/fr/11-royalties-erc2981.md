# ERC-2981 : information de royalties

`royaltyInfo(tokenId, prix)` retourne un bénéficiaire et un montant. Les paramètres peuvent être globaux ou propres à un NFT.
**Exemple :** avec un dénominateur de 10 000 et un taux de 500, une vente de 100 unités donne 5 unités de royalties.
**Piège :** cette interface calcule une information ; elle n'exécute pas le paiement et ne force pas la place de marché à l'honorer.
Le montant retourné utilise la même unité que le prix transmis. ERC-2981 complète un standard de NFT.

[Code](../../contracts/token/common/ERC2981.sol) · [Intégration ERC-721](../../contracts/token/ERC721/extensions/ERC721Royalty.sol) · [Tests](../../test/token/ERC721/extensions/ERC721Royalty.test.js)

[Suite : ERC6909 et permissions fines](12-erc6909.md)
