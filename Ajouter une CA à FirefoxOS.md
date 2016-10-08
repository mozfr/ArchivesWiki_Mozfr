# Comment ajouter une autorité de certification à FirefoxOS

Si vous croisez ce bug https://bugzilla.mozilla.org/show_bug.cgi?id=769178, vous voudrez peut-être ajouter une autorité de certification à la liste de celles reconnues par FirefoxOS.

[[Adding_CA_to_FirefoxOS|English version here]]
autre détails : http://blog.freezetux.net/2014/06/14/Ajout-d-un-CA-%C3%A0-FirefoxOS

## Prérequis 
* Un périphérique FirefoxOS
    * Le fonctionnement avec le simulateur FirefoxOS est laissé en exercice au lecteur
* Outils NSS (principalement certutil)
* Le certificat de l'autorité au format PEM
* La documentation complète des outils NSS : https://developer.mozilla.org/fr/docs/NSS_reference/NSS_tools_:_certutil
* Dans ce qui suit, <RANDOMSTRING> est le nom de votre profil b2g. Il s'agit du seul répertoire qui devrait apparaître :
 `$ adb shell ls /data/b2g/mozilla/`

## Préparation
* Récupérer le trousseau de clefs et certificats du périphérique

 ```
 $ mkdir -p keys && cd keys/
 $ adb pull /data/b2g/mozilla/<RANDOMSTRING>.default/cert9.db .
 $ adb pull /data/b2g/mozilla/<RANDOMSTRING>.default/key4.db .
 ```
 
* Ensuite, définissez un mot de passe vide, sans quoi vous obtiendrez des erreurs du type « certutil: could not authenticate to token NSS Certificate DB.: An I/O error occurred during security authorization. »

    ```
    $ certutil -d sql:. -W
      Enter a password which will be used to encrypt your keys.
      The password should be at least 8 characters long,
      and should contain at least one non-alphabetic character.
    
      Enter new password: 
      Re-enter password: 
    $
    ```

## Ajout

`$ certutil -A -n "<NomCA>" -t "PTCu,PCu,PTuw" -u "V" -d sql:. -i <FichierCA>`

Ceci ajoutera le certificat de l'autorité contenu dans <FichierCA> avec totale confiance passée via le paramètre -t, et sous le nom <NomCA>.

## Vérification
`$ certutil -V -n "<CAName>" -u V -d sql:.`
`certutil: certificate is valid`

Si vous obtenez quoi que ce soit d'autre, cela signifie que cela a échoué.

## Installation
```
$ adb push cert9.db /data/b2g/mozilla/<RANDOMSTRING>.default/
$ adb push key4.db /data/b2g/mozilla/<RANDOMSTRING>.default/
```

Maintenant tout devrait être bon !
