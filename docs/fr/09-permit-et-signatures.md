# Permit et transferts signés

ERC-2612 permet de soumettre une autorisation de dépense signée avec `permit`.
La signature lie notamment bénéficiaire, montant, nonce et échéance ; le domaine EIP-712 la lie au réseau et au contrat.
**Exemple :** signer pour 5 tokens ne les transfère pas. Une transaction soumet l'autorisation, puis `transferFrom` peut la consommer. Un tiers peut payer le gas.
ERC-3009 signe directement un transfert déterminé : cette différence éclaire le paiement `exact` de x402.
**Piège :** l'implémentation ERC-3009 du dépôt porte le préfixe `draft` ; ne pas supposer qu'elle reproduit toutes les particularités d'un token déployé.

[Permit](../../contracts/token/ERC20/extensions/ERC20Permit.sol) · [Tests](../../test/token/ERC20/extensions/ERC20Permit.test.js) · [ERC-3009](../../contracts/token/ERC20/extensions/draft-ERC3009.sol)

[Suite : Tokens de gouvernance](10-gouvernance.md)
