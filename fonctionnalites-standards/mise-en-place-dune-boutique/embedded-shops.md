# Boutique intégrée à votre site web

Cette fonctionnalité vous permet d'offrir la possibilité à vos acheteurs d'acheter directement dans votre site web sur votre boutique Open Food Network.

{% hint style="warning" %}
Cette fonctionnalité est actuellement basée sur une "iframe" (un bout de code qui permet d'intégrer la boutique dans votre site comme vous intégreriez une video Youtube par exemple). Nous avons constaté les limites de cette approche technique, notamment lorsque vos visiteurs naviguent via un terminal mobile : le scroll sur la page est limité à l'iframe, donc il peut parfois être compliqué d'en sortir et de revenir vers le site initial.\
Nous sommes donc en réflexion pour remplacer cette fonctionnalité.

D'ici là, nous ne pouvons garantir l'absence de bugs et recommandons donc de ne pas l'utiliser. 
{% endhint %}

## Pré-requis

### Technologie utilisée pour construire votre site web

La fonctionnalité fonctionne (avec les limites évoquées ci-dessus) sur différents types de site internet, à partir du moment où la technologie utilisée vous permet d'ajouter du code html dans la page où vous souhaitez intégrer la boutique. Wordpress, Wix, Squarespace par exemple permettent cela.

### Sécurité

Open Food Network est une place de marché ce qui implique que des transactions sont effectuées via la plateforme. Cela implique que nos standards de sécurité sont bien plus élevés que pour un site informationnel basique. **Ainsi, si vous ne l'avez pas déjà fait, vous devrez installer un certificat SSL/TLS sur votre site pour que l'intégration fonctionne.**

Vous pouvez obtenir ce type de certificat gratuitement via [Let’s Encrypt](https://letsencrypt.org), ou aux alentours de 10-30€ via d'autres prestataires commerciaux.

### Boutique Open Food Network

Cela parait évident mais c'est toujours mieux en le disant : il faut [créer une boutique](./) sur la plateforme avant de pouvoir l'intégrer dans votre site web. En effet, vous allez avoir besoin de l'URL de cette boutique dans les étapes suivantes.

## Mise en place

**1) Contactez le fournisseur local de la plateforme Open Food Network**

La première étape est de nous contacter afin que nous puissions autoriser votre site à appeler une page depuis la plateforme Open Food Network. Nous aurons besoin de l'URL de votre site internet (ex : monpanierpaysan.com).

**2) Ajoutez un bout de code HTML à votre site**

Voici le bout de code HTML à ajouter à l'endroit où vous souhaitez que la boutique s'affiche :

```
<iframe src=" https://www.openfoodnetwork.be/permalien/shop?embedded_shopfront=true"style="width:100%;min-height:35em"></iframe>
```

**Attention**, à la place ‘permalien’ vous devrez indiquer le permalien de votre boutique (accessible sur les [informations de base](../votre-profil/parametres.md#informations-de-base) de votre entreprise).

A partir de là, vous devriez voir votre boutique Open Food Network dans votre site.

**3) Personnalisation**

En fonction de votre site, il est possible que vous ayez besoin (ou envie) d'ajouter des touches de CSS pour peaufiner le rendu visuel de l'intégration. Cela peut permettre de changer la taille de la fenêtre d'intégration par exemple, éviter d'avoir deux barres de "scrolling", ou autre.

N'oubliez pas de bien tester l'intégration sur une navigation mobile ! Si votre intégration n’apparaît pas bien sur mobile, vous aurez peut-être besoin de quelques adaptations CSS supplémentaires.

## Instructions pour vos visiteurs

### Cookies

Attention, si vos visiteurs n'ont pas accepté les cookies (nécessaires au fonctionnement de l'intégration), ils ne verront pas la page intégrée ! 

