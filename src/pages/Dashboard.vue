<template>
  <div>
    <div class="row">
      <div class="col-12">
        <card type="chart">
          <template slot="header">
            <h3 class="card-title">Projet en équipe de 6 personnes - Développement d'une Application Web de Calcul d'Empreinte Carbone</h3>
            <h5>
              Dans le cadre de l'unité d'enseignement "Projet transversal" (M1if10) du Master 1 Informatique de l'Université Claude Bernard Lyon 1, nous avons collaboré à la création d'une application web de calcul d'empreinte carbone. Mon rôle de développeur backend a inclus l'établissement d'un système d'authentification sécurisé, le développement d'une API fonctionnelle, ainsi que l'implémentation de tests et de documentation. Ce projet a été une opportunité unique pour appliquer nos connaissances académiques dans un contexte professionnel simulé, en mettant l'accent sur la qualité et la sécurité du développement logiciel.
            </h5>

          </template>
          <div >
            <img src="/img/co2.png" width="100%" height="100%" alt="CV" class="cv-image"  ref="cvImage" />
          </div>
        </card>
      </div>
    </div>
    <div class="row">
      <div class="col-lg-4" >
        <card type="chart">
          <template slot="header">
            <h3 class="card-title">Contribution à la librairie python de recherche CDlib</h3>
            <h5 >
              Ce projet vise à enrichir la librairie Python CDlib, spécialisée dans l'analyse des
              communautés dans les réseaux complexes. Les contributions incluent le développement de nouvelles
              visualisations de communautés, l'extension de fonctionnalités existantes et l'amélioration de la
              documentation. L'objectif est de consolider CDlib en tant qu'outil pour l'analyse et la visualisation de
              réseaux dans l'écosystème Python. <a href="/img/projet_cdlib.pdf">Cliquez ici pour consulter le rapport du projet</a>
            </h5>

          </template>
          <div >
            <img  width="100%" height="100%" src="/img/cdlib.png" alt="CV" class="cv-image"  ref="cvImage" />
          </div>
        </card>
      </div>
      <div class="col-lg-4" >
        <card type="chart">
          <template slot="header">
            <h3 class="card-title">Amélioration d'un Chatbot inspiré de ChatGPT : MVC, GRASP, et Tests Automatisés</h3>
            <h5 >
              Le projet consiste à améliorer un chatbot inspiré de ChatGPT en raffinant sa structure de code initiale, en étendant ses fonctionnalités en utilisant les principes MVC et GRASP, en mettant en place des tests automatisés avec JUnit et Maven, et en promouvant le développement piloté par les tests avec GitLab-CI. Il offre une expérience complète du cycle de vie du développement logiciel, avec un accent sur les compétences professionnelles en ingénierie logicielle.
            </h5>

          </template>
          <div >
            <img  width="100%" height="100%" src="/img/eliza.png" alt="CV" class="cv-image"  ref="cvImage" />
          </div>
        </card>
      </div>
      <div class="col-lg-4" >
        <card type="chart">
          <template slot="header">
            <h3 class="card-title">Machine Learning - Prédiction du Succès des Films au Box-Office Local, Étranger et Mondial</h3>
            <h5 >
              Ce projet vise à prédire les revenus domestiques, étrangers et mondiaux des films
              à l'aide de modèles de régression d'arbres de décision. En utilisant un ensemble de
              données détaillé sur les films, les modèles ont été optimisés via la validation croisée et
              GridSearchCV. Les résultats montrent une performance particulièrement élevée pour les
              prédictions mondiales, indiquant que l'approche IA numérique est efficace pour ce type de
              tâche. Le projet est disponible en open-source sur <a href="https://github.com/amineitji/Machine_learning_prediction_movies/">mon GitHub</a>.
           </h5>

          </template>
          <div > 
            <img width="100%" height="100%" src="/img/ml_movies.png"  alt="CV" class="cv-image"  ref="cvImage" />
          </div>
        </card>
      </div>
    </div>
    <div class="row">
      <div class="col-lg-6 col-md-12">
        <card type="chart">
          <template slot="header">
            <h3 class="card-title">Projet en binome - Simulation d’un écosystème</h3>
            <h5 >
              Simulation NetLogo des interactions entre les abeilles, les fleurs, les prédateurs et les ruches dans un environnement dynamique. Chaque agent est caractérisé par des attributs spécifiques qui influent sur son comportement et sa contribution à l'écosystème simulé. L'analyse des comportements individuels des agents permet de mieux comprendre les mécanismes de collecte de pollen, la survie des abeilles et la gestion des ressources au sein des colonies. Bien que la simulation présente certaines limitations, notamment en termes de complexité des interactions et de réalisme météorologique, elle constitue un outil pour étudier les dynamiques écologiques et les stratégies d'adaptation des organismes vivants.
            </h5>

          </template>
          <div >
            <iframe width="100%" height="100%" src="https://www.youtube.com/embed/kZcpo4sGe6g" title="YouTube video player" frameborder="0"  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen  ref="cvVideo"></iframe>
          </div>
        </card>
       
      </div>
      <div class="col-lg-6 col-md-12">
        <card type="chart">
          <template slot="header">
            <h3 class="card-title">Fullstack - Développement d'une Application Web avec Django et Vite.js</h3>
            <h5 >
              Pendant mon stage chez Aneqqis (entreprise dont je suis co-fondateur), j'ai developpé entièrement une application web en utilisant Django pour le backend et Vite.js pour le frontend, incluant également le déploiement final. J'ai mis en place un système d'authentification robuste avec double authentification par email, intégré Stripe pour la gestion sécurisée des paiements, et développé un module automatisé de génération de documents immobiliers.
           </h5>
        </template>
          <div > 
            <iframe width="100%" height="100%" src="https://www.youtube.com/embed/PiKLRnlXitk" title="YouTube video player 2" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen  ref="cvVideo"></iframe>
          </div>
        </card>
      </div>
    </div>
  </div>
</template>