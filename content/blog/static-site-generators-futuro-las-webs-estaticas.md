---
title: Static site generators, 
date: 2020-07-07T17:04:41+06:00
image: images/blog/post-16.jpg
author: Admin
description: "el futuro de las webs estáticas (Hugo, Jekyll, Flask y otros)"
---

### Introducción

En Sitelabs tenemos muy presente que los CMS (gestores de contenido) conforman una gran parte de la web (cerca de un 45%), y la cifra es mucho mayor si hablamos de webs para PYMES, donde WordPress es, de lejos, el sistema de gestión de contenidos más popular. Su ecosistema de plugins, ofreciendo casi cualquier funcionalidad bajo el sol (dentro de las propias limitaciones de la plataforma) lo convierten en la mejor opción a la hora de crear una web de una forma fácil y rápida.

Sin embargo, herramientas como WordPress ofrecen muchas ventajas con un coste que en algunos casos puede convertirse en una gran desventaja: el rendimiento. Viendo este nicho, desarrolladores de todo el mundo han propuesto diferentes soluciones que ofrecen una gestión de contenidos intuitiva sin sacrificar el rendimiento; la gran mayoría de estas herramientas están categorizadas bajo el nombre de generadores de páginas estácticas o static site generators. Veamos cuales son sus características y como pueden contribuir a un desarrollo más fácil y un mejor rendimiento.

# Funcionalidades diversas

La funcionalidad de los generadores de páginas estáticas también varían dependiendo de su objetivo: algunos se limitan a ofrecer las comodidades de las parciales, es decir, separar nuestros archivos HTML en módulos para su reutilización; otros nos dan la opción de definir rutas para nuestras plantillas, es decir, crear URLs «bonitas» y apuntar a nuestras plantillas con las mismas como Guzzle en varios frameworks PHP; y otros nos ofrecen suites completas donde podemos sacar el jugo a opciones como caché y minificación automáticos, jerarquización de páginas o incluso sistema de usuarios database-free. Por norma general, todos los generadores de páginas estáticas se dividen entre los minimalistas y los más equipados, aunque también tenemos que tener en cuenta que algunos son generalistas mientras que otros estan fuertemente «opinionados». Elegir uno u otro depende de las necesidades de cada proyecto así como de los gustos del equipo de desarrolladores.

# Un rendimiento inmejorable

El hecho de prescindir de una base de datos hace que los tiempos de carga sean extremadamente rápidos: para cargar todo el HTML al servidor solo le hace falta leer el contenido del archivo y mandarlo como respuesta. A menudo las páginas que dependen de una base de datos realizan múltiples queries, y cada una de ellas suma latencia a la petición del cliente. Además, al no necesitar más que un servidor web y un lenguaje para el backend, (aunque cada vez surgen más generadores que sólo se basan en lenguajes de cliente y un compilador frontend que lo organiza todo) el alojamiento del sitio web se simplifica y por ende se abarata mucho, permitiéndonos responder muchas más peticiones por segundo y alojar más webs en un mismo servidor, ya que un proceso de mySQL o MongoDB consume muchos recursos mientras se ejecuta.

# Generadores de páginas estáticas especializados

No olvidemos que dependiendo del proyecto que tengamos que crear, existen generadores especializados en un tipo concreto de páginas web. Por ejemplo, GitBook se especializa en generar documentación para nuestros repositorios en Git de forma automatizada, Jekyll se encarga de hacer que publicar y mantener un blog sea muy sencillo y rápido, o Hugo posibilita que el proceso de despliegue de una web sea increíblemente sencillo, ya que genera un ejecutable binario que solamente tendremos que subir al servidor y ya estará funcionando. Aunque existan herramientas como estas especializadas en mejorar la experiencia del usuario en casos concretos, la mayoría de ellas intentan abarcar la mayor cantidad de use cases posibles, siempre dentro de sus limitaciones.

De forma similar a la solución que proponen los generadores de páginas estáticas a los grandes gestores de contenidos, existe una alternativa más ligera a los principales frameworks que se hacen más pesados según evoluciona Internet: los microframeworks. Estos son de gran utilidad para crear microservicios para propósitos específicos. Por ejemplo, si queremos crear una API que conecte con una base de datos y que simplemente muestre y guarde datos en la misma, y intercambiar dichos datos en formato JSON con el cliente (que podría ser, por ejemplo, una app móvil), un microframework sería la apuesta ideal, ya que no consume excesivos recursos y cumple su cometido de forma eficaz y rápida. Dos ejemplos de microframeworks son Flask para Python y Lumen, basado en el framework PHP Laravel.

En Sitelabs creemos que los generadores de páginas son una apuesta segura y que eventualmente desplazarán a los sistema de gestión de contenidos. Sin embargo, el ecosistema de herramientas aún tiene que madurar y diversificarse para convertirse en una alternativade calidad a los grandes proyectos que dominan Internet, como WordPress o Drupal. En los siguientes años veremos como se diversifican las webs estáticas y empiezan a adoptar este enfoque más simple, rápido y seguro.

