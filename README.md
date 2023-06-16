<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

Nws raug nquahu kom nruab nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) ua ntej, thiab tom qab ntawd `direnv allow` tom qab nkag mus rau hauv phau ntawv teev npe ( [tus .envrc](https://github.com/xxai-art/doc/blob/main/.envrc) yuav raug txiav txim siab tom qab nkag mus rau hauv phau ntawv qhia).

The meaning is: Suav translation to Japanese, Korean, English, English translation to all other languages. Yog tias koj tsuas xav txhawb Suav thiab Askiv, koj tuaj yeem sau `zh: en` .

The meaning is: Suav translation to Japanese, Korean, English, English translation to all other languages. Yog tias koj tsuas xav txhawb Suav thiab Askiv, koj tuaj yeem sau `zh: en` .

* [pem hauv ntej-kawg code](https://github.com/xxai-art/web)
* [Cov lus ntim rau lub xaib tag nrho](https://github.com/xxai-art/web/tree/main/i18n)
* [Cov pob lus rau kev nkag mus rau modules](https://github.com/wacpkg/user/tree/main/ui.i18n)
* [Website Multilingual Documentation](https://github.com/xxai-doc)

Cov lus programming pem hauv ntej yog [@w5/coffee_plus](http://npmjs.com/@w5/coffee_plus) , uas ntxiv qee qhov nta raws li cov lus hauv kas fes, saib [./coffee_plus.md](./coffee_plus.md) .

## Internationalization ntawm cov vev xaib thiab cov ntaub ntawv

Ua raws li 3 txoj haujlwm hauv qab no

* [@w5/mdt](https://www.npmjs.com/package/@w5/mdt)

  Lub ntsiab lus yog `.mdt` , koj tuaj yeem siv cov syntax zoo ib yam li `<+ ./coffee_plus/import.js>` xa mus rau cov ntaub ntawv sab nraud, thiab tsim cov cim cim nrog cov lus `.md` .

* [@w5/trmd](https://www.npmjs.com/package/@w5/trmd)

  Markdown txhais lus yuav tsis txhais cov lej thiab txuas, thiab yuav cache cov kab lus txhais. Yog tias qhov kev txhais lus raug hloov kho tab sis cov ntawv qub tsis raug hloov kho, nws rov ua dua yuav tsis sau qhov kev hloov pauv ntawm kev txhais lus.

* [@w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  Cov ntaub ntawv lus rau kev txhais `yaml` tsim cov vev xaib.

### Cov ntaub ntawv txhais lus Automation cov lus qhia

Saib code repository [xxai-art/doc](https://github.com/xxai-art/doc)

Nws raug nquahu kom nruab nodejs, [direnv](https://direnv.net) , [bun](https://github.com/oven-sh/bun) ua ntej, thiab tom qab ntawd `direnv allow` tom qab nkag mus rau hauv phau ntawv teev npe ( [tus .envrc](https://github.com/xxai-art/doc/blob/main/.envrc) yuav raug txiav txim siab tom qab nkag mus rau hauv phau ntawv qhia).

Txhawm rau kom tsis txhob muaj cov cai loj hauv paus txhais ua ntau pua hom lus, kuv tau tsim ib lub hauv paus cais rau txhua hom lus thiab tsim ib lub koom haum los khaws cov cai hauv paus.

Kev teeb tsa ib puag ncig hloov pauv `GITHUB_ACCESS_TOKEN` thiab tom qab ntawd khiav [create.github.coffee](https://github.com/xxai-art/doc/blob/main/create.github.coffee) yuav cia li tsim cov code repository.

Tau kawg, koj tuaj yeem muab tso rau hauv lub hauv paus code.

Cov ntawv txhais lus siv [run.sh](https://github.com/xxai-art/doc/blob/main/run.sh)

Tsab ntawv code yog txhais raws li nram no:

[bunx](https://bun.sh/docs/cli/bunx) yog qhov hloov pauv rau npx, uas yog nrawm dua. Tau kawg, yog tias koj tsis muaj bun ntsia, koj tuaj yeem siv `npx` hloov.

`bunx mdt zh` renders `.mdt` hauv zh directory as `.md` , saib 2 cov ntaub ntawv txuas hauv qab no

* [coffee_plus.mdt](https://github.com/xxai-doc/zh/blob/main/coffee_plus.mdt)
* [coffee_plus.md](https://github.com/xxai-doc/zh/blob/main/coffee_plus.md)

`bunx i18n` yog tus lej cim rau kev txhais lus (yog tias koj tsuas muaj `nodejs` ntsia, tab sis `bun` thiab `direnv` tsis tau nruab, koj tuaj yeem khiav `npx i18n` los txhais).

Nws yuav parse [i18n.yml](https://github.com/xxai-art/doc/blob/main/i18n.yml) , kev teeb tsa ntawm `i18n.yml` hauv daim ntawv no yog raws li nram no:

```
en:
zh: ja ko en
```

The meaning is: Suav translation to Japanese, Korean, English, English translation to all other languages. Yog tias koj tsuas xav txhawb Suav thiab Askiv, koj tuaj yeem sau `zh: en` .

Qhov kawg yog [gen.README.coffee](https://github.com/xxai-art/doc/blob/main/gen.README.coffee) , uas rho tawm cov ntsiab lus ntawm lub ntsiab lus tseem ceeb thiab thawj subtitle ntawm txhua hom lus `README.md` los tsim ib qho kev nkag `README.md` . Cov cai yooj yim heev, koj tuaj yeem saib nws tus kheej.

Google API yog siv rau kev txhais lus dawb. Yog tias koj nkag tsis tau Google, thov teeb tsa thiab teeb tsa lub npe, xws li:

```
export https_proxy=http://127.0.0.1:7890 http_proxy=http://127.0.0.1:7890 all_proxy=socks5://127.0.0.1:7890
```

Cov ntawv txhais lus yuav tsim kom muaj cov ntaub ntawv txhais lus hauv `.i18n` , thov xyuas nws nrog `git status` thiab ntxiv rau hauv qhov chaw cia code kom tsis txhob rov rov txhais dua.

Thov khiav `bunx i18n` txhua zaus koj hloov kho cov lus txhais kom hloov kho lub cache.

Yog tias cov ntawv qub thiab cov lus txhais tau hloov pauv tib lub sijhawm, lub cache yuav tsis meej pem, yog li yog tias koj xav hloov kho, koj tuaj yeem hloov kho ib qho, thiab tom qab ntawd khiav `bunx i18n` los hloov kho lub cache.
