---
type: slide
title: YunoHost JDLL 2021
slideOptions:
  theme: white
  transition: slide
  width: 1280
  height: 1080
  margin: 0.01
---

<img src="https://yunohost.org/_images/ynh_logo_black_300dpi.png" width="200px" class="plain">

## De l'auto-hébergement<br /> à l'élevage de CHATONS

### Journées du Logiciel Libre
### 2021-04-04 - 11:00 CET

----

<img src="./uploads/upload_ab05064b3f99b3b99703cc6f72840112.jpg" width="100px" class="plain"> 

`tituspijean`

---

## Sommaire

1. Pourquoi s'auto-héberger ?
2. YunoHost
3. Côté administrateur ($\hookleftarrow$ c'est vous !)
4. Côté technique
5. Côté communauté

---

## Introduction

----

### Qui possède vos données ?

* Votre disque dur, clé USB, ...
* Fournisseurs de services (*drive, *box)

----

<!-- .slide: data-background-image="./uploads/upload_e991f29ebf5cae9b1f6f7fa4ed6db8c7.jpg" data-background-size="contain" data-background-color="black" -->

<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />
<br />

### Envoi centralisé de données vers le nuage
<!-- .element style="color: white;" -->
*Incendie d'un centre de données d'OVH,
à Strasbourg, mars 2021*
<!-- .element style="color: white;" -->

----

<img src="./uploads/upload_e9f1516057d8ba9597fd14a016cdd44b.png" height="80%" class="plain" />
<small>Illustration par JimboJoe</small>

----

### Vie privée

Est-il bien raisonnable que notre garagiste connaisse...
- avec qui on covoiture ;
- ce que l'on écoute à la radio ;
- nos trajets quotidiens et exceptionnels ;
- et moultes autres choses bien personnelles...

sous prétexe que c'est pour rendre un service "plus personnalisé",
et en profiter pour revendre notre "profil" aux constructeurs automobiles ou autres vendeurs de sapins sent-bon ?
<!-- .element class="fragment" -->

*Ici, le garagiste, c'est n'importe quel GAFAM.*
<!-- .element class="fragment" -->

----

Qu'ont en commun

*L'origine du monde* de Courbet,
<!-- .element class="fragment" -->

des oignons,
<!-- .element class="fragment" -->

et D. Trump ?
<!-- .element class="fragment" -->

### La liberté d'expression <!-- .element class="fragment" -->

----

* Possession des données
* Décentralisation
* Vie privée
* Liberté d'expression

## $\implies$ Motivations à l'auto-hébergement

----

## Comment s'auto-héberger ?
### Le matériel

<img src="https://yunohost.org/user/images/virtualbox.png
" height="200px" class="plain fragment" /> <img src="https://yunohost.org/user/images/raspberrypi.jpg
" height="200px" class="plain fragment" /> <img src="https://yunohost.org/user/images/computer.png
" height="200px" class="plain fragment" /> <img src="https://yunohost.org/user/images/vps.png
" height="200px" class="plain fragment" />

----

## Comment s'auto-héberger ?
### Le logiciel

|             | Alternatives libres |
| ----------- | -------- |
| Twitter | <img src="./uploads/upload_f6fa5b055c5172f7c1d3101c5d149274.png" height="50px" class="plain" /> Mastodon |
| Dropbox, GDrive... | <img src="./uploads/upload_37dc6043f0e3f04d3105752d1a35ffca.png" height="50px" class="plain" /> Nextcloud |
| Office Online | <img src="./uploads/upload_8be3daead4b3a7c8add5c576f50bc09d.png" height="50px" class="plain" /> Cryptpad |
| Tout système de domotique | <img src="./uploads/upload_6c1b830d679ff9bf6cf0298176980e8b.png" height="50px" class="plain" /> Home Assistant |
| Messenger, Whatsapp, Wechat... | <img src="./uploads/upload_8251d4b5cee69a53c8de8de38c839fba.png" height="50px" class="plain" /> |
<!-- .element style="width: 90%" -->

**... chacun avec ses propres prérequis
et instructions d'installation**

---

<!-- .slide: data-background-image="https://64.media.tumblr.com/4b3b0287ca43ce1021340cd692f65f9f/tumblr_mj7iufgKNi1qghl49o1_500.gifv" -->

<img src="./uploads/upload_f665f0adec32d34e1e9cfc7954b4505c.png" class="fragment plain" />

<img src="./uploads/upload_03fba19df10fad1c8c8235157cb864a6.gif" height="500px" class="fragment plain" />

----

## Il est *nécessaire* de rendre l'administration de serveurs __simple__

----

<img src="https://yunohost.org/_images/ynh_logo_black_300dpi.png" alt="YunoHost" class="plain" width="300px" /> <span class="fragment fade-out" >vs.?</span> <span class="fa fa-heart fragment" style="color: red;"></span> <img src="./uploads/upload_9ee7181534d2bae985464754764539c7.png" alt="CHATONS" class="plain" height="400px" />

> CHATONS est le **Collectif des Hébergeurs Alternatifs, Transparents, Ouverts, Neutres et Solidaires**. Ce collectif vise à rassembler des structures proposant des services en ligne libres, éthiques et décentralisés.
https://chatons.org
https://wiki.chatons.org/doku.php/yunohost
<!-- .element style="width: 90%" -->

----

# <img src="./uploads/upload_68522fd4880f25b1a5f798b9c1bf5b5c.png" alt="YunoHost" height="90px" class="plain" />, c'est quoi ?
- <img src="https://www.debian.org/logos/openlogo-nd-100.png" alt="Debian" height="50px" class="plain" /> une distribution Debian
<!-- .element class="fragment" style="width: 100%" -->
- <span class="fa fa-wrench"></span> une interface d'administration simple
<!-- .element class="fragment" style="width: 100%" -->
- <span class="fa fa-envelope"></span><span class="fa fa-comments"></span> des services fonctionnels dès l'installation
<!-- .element class="fragment" style="width: 100%" -->
- <span class="fa fa-globe"></span> des noms de domaines gratuits et automatiquement configurés (`.ynh.fr`, `.nohost.me`, `.noho.st`)
<!-- .element class="fragment" style="width: 100%" -->
- <span class="fa fa-cubes"></span> plus de 200 applications installables en quelques clics 
<!-- .element class="fragment" style="width: 100%" -->
- <span class="fa fa-lock"></span> un portail de connexion pour les personnes inscrites
<!-- .element class="fragment" style="width: 100%" -->
- <span class="fa fa-key"></span> un système de permissions pour contrôler les accès aux apps
<!-- .element class="fragment" style="width: 100%" -->
- <span class="fa fa-stethoscope"></span> un système de diagnostic pour déboger tout ça
<!-- .element class="fragment" style="width: 100%" -->

----

## YunoHost, côté utilisateur/administrateur
### Une petite démo ?

https://demo.yunohost.org

---

## YunoHost, côté technique

----

### Installable en moins d'une heure

<img src="https://yunohost.org/user/images/virtualbox.png
" height="200px" class="plain" /> <img src="https://yunohost.org/user/images/raspberrypi.jpg
" height="200px" class="plain" /> <img src="https://yunohost.org/user/images/computer.png
" height="200px" class="plain" /> <img src="https://yunohost.org/user/images/vps.png
" height="200px" class="plain" />

----

### Automatisation des tâches de sysadmin

Accessibles via l'interface web ou la ligne de commande

<div style="width: 100%;">
<img src="./uploads/upload_5a94ecd08e991359407b151987fe8b2c.png" height="600px" class="" /> <img src="./uploads/upload_c46014db9c0ef00f3d6890243cf248ae.png" height="600px" class="plain" /> 
</div>

----

### Les applications

Des fichiers de description, de configuration,
et des scripts Bash pour laisser la magie opérer.

<img src="./uploads/upload_3814b802aaafbe4e32a45891a59f9f40.png" height="600px" class="" />
<img src="./uploads/upload_f4f13b2e4dd443c5df8c0ba1916b3d19.png" height="600px" class="" />

\+ un système de tests automatisés pour aider les *packagers*

----

### Feuille de route

- 4.2 (en test)
    - Passage de Python 2 à Python 3
    - Réécriture de la webadmin
    - Import d'utilisateurs (<span class="fa fa-heart" style="color: red; height=30px;"></span> <img src="https://pijean.ovh/doc/uploads/upload_9ee7181534d2bae985464754764539c7.png" alt="CHATONS" class="plain" height="50px" />)
    - Simplification de la post-installation
- 4.3
    - Formulaire d'inscription des utilisateurs (<span class="fa fa-heart" style="color: red; height=30px;"></span> <img src="https://pijean.ovh/doc/uploads/upload_9ee7181534d2bae985464754764539c7.png" alt="CHATONS" class="plain" height="50px" />)
    - Une configuration améliorée des apps, après leur installation
- et encore...
    - Fédération de serveurs

---

## YunoHost, côté communauté

----

### ~5000 instances YunoHost

----

### Plus de 200 applications

![](./uploads/upload_cd63cb311e82c705f84de09f1d3ae4d5.png)

208 pleinement fonctionnelles sur 236 testées
383 en tout dans les tuyaux

----

### Nous trouver

* Le site web de YunoHost : https://yunohost.org
* Le forum pour les annonces et l'entraide : https://forum.yunohost.org
* Des salons de discussion d'entraide pour le support, le *packaging* d'apps, le développement : [Matrix/IRC](https://yunohost.org/fr/chat_rooms)
* La documentation : https://yunohost.org/docs

<span class="fa fa-heart" style="color: red; height=30px;"></span> bénévoles
<span class="fa fa-heart" style="color: red; height=30px;"></span> contributeurs (Python, UX, HTML, CSS, JS, Bash, ...)

----

# <span class="fa fa-heart" style="color: red; height=30px;"></span> Nos soutiens

![](./uploads/upload_020660247dbd50f71b8b0e151f211218.png)

----

## Dans les coulisses...

* Présentation diffusée avec [Galène](https://galene.org)...
* ... faite avec [Reveal.js](https://revealjs.com/) sur [HedgeDoc](https://hedgedoc.org/)...
* ... que j'accède avec mon propre VPN avec [WireGuard](https://wireguard.com)...
* ... le tout auto-hébergé sur mon serveur [<img src="./uploads/upload_68522fd4880f25b1a5f798b9c1bf5b5c.png" alt="YunoHost" height="50px" class="plain" />](https://yunohost.org)

---

# Avez-vous des questions ?