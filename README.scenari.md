# Fork de xslt_polyfill pour Scenari

Le fork est utilisé pour produire le WASM d'appel à libxslt.
Le polyfill Javascript de ce projet n'est pas utilisé.
Une version a été réimportée et fortement simplifiée pour s'intégrer dans le cœur de Scenari.

La principale modification est la production du code binaire du WASM dans un fichier `.wasm` à part. Il n'est plus intégré dans le loader.
Les fichiers WASM produits dans le dossier dist ont été renommés en `xsltPolyfillWasm.(js|wasm)` et sont à copier dans `/Wui_Commons/lib/commons/xslt/`.
