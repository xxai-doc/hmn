<p align="center"><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/logo.svg"/></a><br/><a href="https://xxai.art"><img src="https://cdn.jsdelivr.net/gh/xxai-art/doc/xxai.svg"/></a></p><p align="center"><a href="https://github.com/xxai-art/doc#readme"><img alt="I18N" src="https://cdn.jsdelivr.net/gh/wactax/img/t.svg"/></a>　<a href="https://groups.google.com/u/0/g/xxai-art"><img alt="Google Groups" src="https://cdn.jsdelivr.net/gh/wactax/img/g-groups.svg"/></a></p>

# xxAI.art

Ib feem ntawm lub vev xaib code yog qhib qhov chaw, txais tos los pab txhim kho kev txhais lus.

## pem hauv ntej-kawg code

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

  Markdown txhais lus yuav tsis txhais cov lej thiab txuas, thiab yuav cache cov kab lus txhais. Yog tias qhov kev txhais lus raug hloov kho tab sis cov ntawv qub tsis raug hloov kho, nws rov ua dua yuav tsis overwrite qhov kev hloov kho ntawm kev txhais lus.

* [@w5/i18n](https://www.npmjs.com/package/@w5/i18n)

  Cov ntaub ntawv lus rau kev txhais `yaml` tsim cov vev xaib.
