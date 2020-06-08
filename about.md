---
layout: about
title: "about"
---

Aquest site ha sigut fet des de Barcelona durant el mes de maig per un aficionat que li agrada programar i des del confinament de la COVID-19. El site esta fet amb **Jekyll** i és molt útil per poder organitzar continguts de vídeo del YouTube en format de **col·leccions per curs** per veure'ls en ordinador de sobretaula o tablet.


### Disseny

Consisteix en una presentació per mostrar **les lliçons** agrupades per **mòduls** o cursos,  amb l'estil dels desenvolupadors de [vuemastery.com](https://www.vuemastery.com/) o [edX](https://www.edx.org/). 

### Pujar continguts

Per pujar continguts només cal crear **un arxiu per curs** i **un arxiu per lliçó**. La plantilla de Jekyll fa la resta: agrupa totes les lliçons del curs, les mostra ordenades i paginades. 

### Funcionament

El sistema **Jekyll** funciona a partir d'unes plantilles i uns scripts, que a partir d'uns arxius que nosaltres creeem
d'una manera molt simple,  genera pàgines estàtiques. Aquests sistemes s'anomenen **generadors de pàgines estàtiques** *(Static Pages Generators)*. **Jekyll** és un de [molts](https://www.staticgen.com/) generadors de pàgines estàtiques. 

### Per què fer-ho amb Jekyll?

Perquè és una sol·lució a la necessitat d'allotjar continguts ordenats, actualitzables, sense bases de dades, que puguin ser generats des de qualsevol plataforma amb un simple editor de textos. Els *sites* poden ser allotjats gratuitament al **Gitlab** o al **GitHub** i poden ser copiats i replicats.

El resultat és possible perquè s'ha fet amb **codi lliure**, és a dir, eines que **no es poden vendre** i desenvolupades per mil·lers de persones. Sabies que la majoria d'ordinadors del món funcionen amb el **sistema operatiu lliure** [GNU/Linux](https://www.gnu.org/)?

<video style="width: 100%;" controls="controls" poster="//static.fsf.org/nosvn/FSF30-video/fsf30-poster.png" crossorigin="anonymous">
<source src="//static.fsf.org/nosvn/FSF30-video/FSF_30_720p.webm" type="video/webm">
<track kind="subtitles" label="Català" srclang="ca" src="https://raw.githubusercontent.com/iiioxoiii/translations/master/FSF_30_ca.vtt" default="default">
<track kind="subtitles" label="English" srclang="en" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.en.vtt" default="default">
<track kind="subtitles" label="Spanish" srclang="es" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_es.vtt">
<track kind="subtitles" label="French" srclang="fr" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.fr.vtt">
<track kind="subtitles" label="German" srclang="en" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.de.vtt">
<track kind="subtitles" label="русский" srclang="ru" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.ru.vtt">
<track kind="subtitles" label="italiano" srclang="it" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.it.vtt">
<track kind="subtitles" label="português" srclang="pt" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.pt.vtt">
<track kind="subtitles" label="српски" srclang="sr" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.sr.vtt">
<track kind="subtitles" label="fārsi" srclang="fa" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.fa.vtt">
<track kind="subtitles" label="nederlands" srclang="nl" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.nl.vtt">
<track kind="subtitles" label="magyar" srclang="hu" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.hu.vtt">
<track kind="subtitles" label="svenska" srclang="se" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.se.vtt">
<track kind="subtitles" label="română" srclang="ro" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.ro.vtt">
<track kind="subtitles" label="lietuvių" srclang="lt" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.lt.vtt">
<track kind="subtitles" label="hebrew" srclang="lt" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.he.vtt">
<track kind="subtitles" label="português do Brasil" srclang="pt-br" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.pt-br.vtt">
<track kind="subtitles" label="chinese" srclang="lt" src="//static.fsf.org/nosvn/FSF30-video/captions/FSF_30_720p.zh-cn.vtt">
</video>




### Com puc instal·lar-me aquest sistema?

Cal descarregar-se el contingut d'aquest respositori, adaptar els continguts al gust i tornar-lo a pujar al vostre repositori.

### Quins arxius haig d'editar per crear el meu *site*?

Bàsicament cal editar els continguts dels arxius: \_data/cursos.yml, \_data/menu.yml, \_config.yml. 

**_data/cursos.yml**

Els cursos que apareixen a la pàgina principal es generen a partir d'esquemes com el aquest:

<div class="hljs" style="width: 800px;"><pre style="
    margin-top: 0px;
    margin-bottom: 0px;
"><code class="plaintext" >
   - nom: "El Mamut Traçut (I)"
  imatge: "images/elmamut.svg"
  etiqueta: "Mostra del bo i millor"
  llibre: "9 videos"
  rellotge: "43 minuts"
  ratlletes: "Master"
  descripcio: "Primer bloc de bandes del segell de música «El Mamut Traçut».El segell està format per grups essencials
              de l'escena independent catalana i també per bandes internacionals." 
  urlprimerallico: "les-atxes/"
 </code></pre>
</div>

Aquest esquema s'interpreta de la següent manera:
![](/images/captura01.png)


**_data/menu.yml**

Els links de la part superior del site.

<div class="hljs" style="width: 800px;"><pre style="
    margin-top: 0px;
    margin-bottom: 0px;
">
	<code class="plaintext">
- pagina: inici 
  url: /video-classroom-fp/

- pagina: moodle
  url: https://educaciodigital.cat/ea-llotja/moodle/

- pagina: about
  url: /video-classroom-fp/
  </code>
</pre>
</div>


Això s'interpreta aixi:

![](/images/capturabar.png)




**_config.yml**

L'arxiu de configuració on s'especifiquen dades com el nom, email, el logo i la url del lloc. És molt important fixar-se tant en la *url* com amb la *baseurl* per fer un desplegament correcte.

<div class="hljs" style="width: 800px;">
<pre style="
    margin-top: 0px;
    margin-bottom: 0px;
"><code class="plaintext">
url: "https://github.com/iiioxoiii/" # La url del teu repositori configurat com Github Page.
baseurl: "/video-classroom-fp" # base url del repositori. 

title: "Video-Classroom-fp" # the name of your site, e.g. ACME Corp.

siteimage: "/images/vuemastery.svg" ## Icona de la esquerra del site

email: "formacioalescola@xtec.cat" ## e-mail 
author: "FormacioProfessional" ## nom de l'autor

## Cursos
collections:
  lessons:
    output: true
    permalink: /:name/
</code></pre>
</div>

### I les «lliçons»? Com puc crear-les?

Per cada lliçó cal crear un arxiu amb extensió **.md** dins la carpeta **_lessons** com es pot veure en el següent exemple:

<div class="hljs" style="width: 800px;">
<pre style="
    margin-top: 0px;
    margin-bottom: 0px;
">
	<code class="plaintext">
---
layout: lessons
title: "Capità Pilgrim" 
curs: "El Mamut Traçut (II)"
lessonnumber: 4
minuts: 3 min
video-url: "https://www.youtube.com/embed/ZjsVd5YpWbI"
 ---

Capità Pilgrim és un trio d’indie-punk-cançó d’autor, o el que sigui. 
Actualment som el Marc Tormo (baterista), lo Víctor Vallejo (baix i veus) i el Jordi 
Morata (guitarra i veu). Anteriorment, en Pablo Ríos (baix i veus) i el Rafel Morata 
(baix i veus) han format part de l’estol. Aviadet, nou disc “Corbs”

Em co-editat el seu disc “Corbs” a mitges amb No Me’n Records i Bestiar Netlabel.

[www.nomenrecords](http://nomenrecords.com/bandes/futura/capita-pilgrim/) 

</code></pre></div>

Aquesta entrada s'interpreta [així](/video-classroom-fp/el-mamut-tracut-2-capita-pilgrim/)

El primer valor no cal tocar-lo. El títol es el nom de la lliçó, el curs ha de ser **el mateix nom** al qual pertany la lliçó, el número (també és necessari i serveix perquè el Jekyll ordeni les lliçons), els minuts i la url del **YouTube**. A sota es posa el contingut en format [markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

Es recomana anomenar tots els arxius **d'un mateix curs amb un prefix** per poder-los distingir amb facilitat.

### Puc afegir més pàgines o crear un *blog*?

Sí. **Jekyll** és molt versàtil i disposa de moltes opcions. Es poden publicar post a l'estil d'un bloc o crear més pàgines sense gaires dificultats. 

### Es pot dir que també és un *blog*?

Sí. A més, amb el **Jekyll** tenim la possibilitat [d'importar continguts ](https://import.jekyllrb.com/) de bases de dades de molts gestors de continguts, com Wordpress, Drupal, Joomla, Behance entre d'altres.

