En general, quand nous faisons face a un programme inconnu, il convient de proceder a une analyse rapide ou approfondie. La duree et la portee de l'analyse dependra de nous rasource et le temps que nous puissions y accorder.

NB: Il convient aussi de consulter les loie locales a propos des IP et le desassemblage et analyse.
Dans certains etats, etant juste en possession de ses outils constitue un crime. 


L'analyse d'un logiciel inconnu constituera a 2 etapes: l'analyse statique et l' analyse dynamique

        I: Static analysis

Cette etape constituera  a analyser le programme ou le logiciel sans pour autant le declencher.

        1. Identifier le programme

a: Recuperer l'empreinte du programm

work$ md5sum ETH\ Seed\ \&\ Keys\ Converter\ @ai_wallets.zip 
3a132e8c1f71226388d8f2ac04ce702b  ETH Seed & Keys Converter @ai_wallets.zip
work$ 

b: Nous ferons de meme pour le contenu de l'archive
TH Seed & Keys Converter @ai_wallets$ md5sum *
d094850c4d40465e86b2b2bccfbcc55b  ETH Seed & Keys Converter.exe
883f0038801554198924f66d05558460  Read Me!.txt
ETH Seed & Keys Converter @ai_wallets$ 


Note: A partir de ces md5sum, nous pouvons rechercher sur google, virustotal,et autres sans leur envoyer le contenu du program. La fois passe quand jai teste le md5sum, le program etait inconnu. Mais il parait que le site a anlyse le programme il ya 15 heures et que 3 engins l'ont trouve suspect.

work$ unzip -v ETH\ Seed\ \&\ Keys\ Converter\ @ai_wallets.zip 
Archive:  ETH Seed & Keys Converter @ai_wallets.zip
 Length   Method    Size  Cmpr    Date    Time   CRC-32   Name
--------  ------  ------- ---- ---------- ----- --------  ----
       0  Stored        0   0% 2025-12-31 07:26 00000000  ETH Seed & Keys Converter @ai_wallets/
52955710  Defl:N 52534961   1% 2025-12-31 07:17 240275b7  ETH Seed & Keys Converter @ai_wallets/ETH Seed & Keys Converter.exe
    3208  Defl:N     1443  55% 2025-12-31 09:02 bf490dff  ETH Seed & Keys Converter @ai_wallets/Read Me!.txt
--------          -------  ---                            -------
52958918         52536404   1%                            3 files
work$ 

La commande unzip -v indiue que le document contient 2 fichiers: "Read Me!.txt" et "ETH Seed & Keys Converter.exe". 
Il semble aussi que le programme a ete cree le 31 dec 2025.


c: Approfondir l'anylyse statiqu

Les details a ce niveau seront similaire a ce que vous trouvez sur cette page: 
https://www.virustotal.com/gui/file/91c2fe7ab19801f4c721cad403689bb266c491a4a413a044de2d3e0a7ee5d69e/details

Des logiciels qui pourront aider:
detecteasy, peid, ghydra idpro, hexray...







        II: Dynamic analysis


L'analyse dynamique consistera a declencher le program dans un environnement plus ou moins controle.


Cela permettra d'observer:
    les requestes sur le net que le logiciel effectue (instructions recues ou messages relayes a au centre de commande)
    les fichiers ou programmmes qu'il touche (ouvre, modifie ou supprime) (persistence possible)
    les changement au cote du registres(utilise pour persistence)





