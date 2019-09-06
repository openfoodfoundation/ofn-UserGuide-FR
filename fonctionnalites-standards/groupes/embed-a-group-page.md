# Intégrer une page groupe à un site web

Cette fonctionnalité vous permet de naviguer au sein d'une page groupe d'Open Food Network depuis votre propre site web. Cette page décrit comment procéder pas à pas.

## Pré-requis

### Technologie utilisée pour construire votre site web <a id="technologie-utilisee-pour-construire-votre-site-web"></a>

La fonctionnalité fonctionne sur différents types de site internet, à partir du moment où la technologie utilisée vous permet d'ajouter du code html dans la page où vous souhaitez intégrer la boutique. Wordpress, Wix, Squarespace, par exemple, permettent cela.

### Sécurité

Open Food Network est une place de marché ce qui implique que des transactions sont effectuées via la plateforme. Cela implique que nos standards de sécurité sont bien plus élevés que pour un site informationnel basique. **Ainsi, si vous ne l'avez pas déjà fait, vous devrez installer un certificat SSL/TLS sur votre site pour que l'intégration fonctionne.**

Vous pouvez obtenir ce type de certificat gratuitement via [Let’s Encrypt](https://letsencrypt.org/), ou aux alentours de 10-30€ via d'autres prestataires commerciaux.

### Groupe Open Food Network

Cela parait évident mais c'est toujours mieux en le disant : il faut [créer un groupe](create-group-page.md) sur la plateforme avant de pouvoir l'intégrer dans votre site web. En effet, vous allez avoir besoin de l'URL de ce groupe dans les étapes suivantes.

## Mise en place

**1\) Contactez le fournisseur local de la plateforme Open Food Network**

La première étape est de nous contacter afin que nous puissions autoriser votre site à appeler une page depuis la plateforme Open Food Network. Nous aurons besoin de l'URL de votre site internet \(ex : monpanierpaysan.com\).

**2\) Ajouter un bout de code HTML à votre site**

Voici le bout de code HTML à ajouter à l'endroit où vous souhaitez que la page groupe s'affiche :

```text
<iframe src="/groups/flavour-crusader?embedded_shopfront=true"style="width:100%;min-height:35em"></iframe>
```

**Attention**, à la place ‘flavour-crusader’ vous devrez indiquer le permalien que vous avez choisi à l'étape de création du groupe.

A partir de là, vous devriez voir votre page groupe dans votre site.

**3\) Personnalisation**

En fonction de votre site, il est possible que vous ayez besoin \(ou envie\) d'ajouter des touches de CSS pour peaufiner le rendu visuel de l'intégration. Cela peut permettre de changer la taille de la fenêtre d'intégration par exemple.

N'oubliez pas de bien tester l'intégration sur une navigation mobile ! Si votre intégration n’apparaît pas bien sur mobile, vous aurez peut-être besoin de quelques adaptations CSS supplémentaires.

## Instructions pour vos visiteurs

### Cookies

Attention, si vos visiteurs n'ont pas accepté les cookies \(nécessaires au fonctionnement de l'intégration\), ils ne verront pas la page intégrée ! 



