<template>
  <div>
    <div class="row">
      <div class="col-12">
        <card type="chart">
          <template slot="header">
            <h3 class="card-title">Projet en équipe de 6 personnes - Développement d'une Application Web de Calcul d'Empreinte Carbone</h3>
            <h5 class="card-category">
              Dans le cadre de l'unité d'enseignement "Projet transversal" (M1if10) du Master 1 Informatique de l'Université Claude Bernard Lyon 1, nous avons collaboré à la création d'une application web de calcul d'empreinte carbone. Mon rôle de développeur backend a inclus l'établissement d'un système d'authentification sécurisé, le développement d'une API fonctionnelle, ainsi que l'implémentation de tests et de documentation. Ce projet a été une opportunité unique pour appliquer nos connaissances académiques dans un contexte professionnel simulé, en mettant l'accent sur la qualité et la sécurité du développement logiciel.
            </h5>

          </template>
          <div class="chart-area">
            <img src="/img/co2.png" width="100%" height="175%" alt="CV" class="cv-image" @load="adjustCardWidth" ref="cvImage" />
          </div>
        </card>
      </div>
    </div>
    <div class="row">
      <div class="col-lg-4" :class="{ 'text-right': isRTL }">
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
          <div class="chart-area">
            <img src="/img/cdlib.png" alt="CV" class="cv-image" @load="adjustCardWidth" ref="cvImage" />
          </div>
        </card>
      </div>
      <div class="col-lg-4" :class="{ 'text-right': isRTL }">
        <card type="chart">
          <template slot="header">
            <h3 class="card-title">Amélioration d'un Chatbot inspiré de ChatGPT : MVC, GRASP, et Tests Automatisés</h3>
            <h5 >
              Le projet consiste à améliorer un chatbot inspiré de ChatGPT en raffinant sa structure de code initiale, en étendant ses fonctionnalités en utilisant les principes MVC et GRASP, en mettant en place des tests automatisés avec JUnit et Maven, et en promouvant le développement piloté par les tests avec GitLab-CI. Il offre une expérience complète du cycle de vie du développement logiciel, avec un accent sur les compétences professionnelles en ingénierie logicielle.
            </h5>

          </template>
          <div class="chart-area">
            TODO : rajouter une image du projet
            <!-- <img src="/img/cdlib.png" alt="CV" class="cv-image" @load="adjustCardWidth" ref="cvImage" /> -->
          </div>
        </card>
      </div>
      <div class="col-lg-4" :class="{ 'text-right': isRTL }">
        <card type="chart">
          <template slot="header">
            <h3 class="card-title">Projet en binome - Simulation d’un écosystème</h3>
            <h5 >
              Simulation NetLogo des interactions entre les abeilles, les fleurs, les prédateurs et les ruches dans un environnement dynamique. Chaque agent est caractérisé par des attributs spécifiques qui influent sur son comportement et sa contribution à l'écosystème simulé. L'analyse des comportements individuels des agents permet de mieux comprendre les mécanismes de collecte de pollen, la survie des abeilles et la gestion des ressources au sein des colonies. Bien que la simulation présente certaines limitations, notamment en termes de complexité des interactions et de réalisme météorologique, elle constitue un outil pour étudier les dynamiques écologiques et les stratégies d'adaptation des organismes vivants.
            </h5>

          </template>
          <div class="chart-area">
            <iframe width="100%" height="100%" src="https://www.youtube.com/embed/kZcpo4sGe6g" title="YouTube video player" frameborder="0" class="cv-image" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen @load="adjustCardWidth" ref="cvVideo"></iframe>
          </div>
        </card>
      </div>
    </div>
    <div class="row">
      <div class="col-lg-6 col-md-12">
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
          <div class="chart-area"> 
            <img src="/img/ml_movies.png" alt="CV" class="cv-image" @load="adjustCardWidth" ref="cvImage" />
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
          <div class="chart-area"> 
            <iframe width="100%" height="100%" src="https://www.youtube.com/embed/PiKLRnlXitk" title="YouTube video player 2" frameborder="0" class="cv-image" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen @load="adjustCardWidth" ref="cvVideo"></iframe>
          </div>
        </card>
      </div>
    </div>
  </div>
</template>
<script>
import LineChart from "@/components/Charts/LineChart";
import BarChart from "@/components/Charts/BarChart";
import * as chartConfigs from "@/components/Charts/config";
import TaskList from "./Dashboard/TaskList";
import UserTable from "./Dashboard/UserTable";
import config from "@/config";

export default {
  components: {
    LineChart,
    BarChart,
    TaskList,
    UserTable,
  },
  data() {
    return {
      bigLineChart: {
        allData: [
          [100, 70, 90, 70, 85, 60, 75, 60, 90, 80, 110, 100],
          [80, 120, 105, 110, 95, 105, 90, 100, 80, 95, 70, 120],
          [60, 80, 65, 130, 80, 105, 90, 130, 70, 115, 60, 130],
        ],
        activeIndex: 0,
        chartData: {
          datasets: [{}],
          labels: [
            "JAN",
            "FEB",
            "MAR",
            "APR",
            "MAY",
            "JUN",
            "JUL",
            "AUG",
            "SEP",
            "OCT",
            "NOV",
            "DEC",
          ],
        },
        extraOptions: chartConfigs.purpleChartOptions,
        gradientColors: config.colors.primaryGradient,
        gradientStops: [1, 0.4, 0],
        categories: [],
      },
      purpleLineChart: {
        extraOptions: chartConfigs.purpleChartOptions,
        chartData: {
          labels: ["JUL", "AUG", "SEP", "OCT", "NOV", "DEC"],
          datasets: [
            {
              label: "Data",
              fill: true,
              borderColor: config.colors.primary,
              borderWidth: 2,
              borderDash: [],
              borderDashOffset: 0.0,
              pointBackgroundColor: config.colors.primary,
              pointBorderColor: "rgba(255,255,255,0)",
              pointHoverBackgroundColor: config.colors.primary,
              pointBorderWidth: 20,
              pointHoverRadius: 4,
              pointHoverBorderWidth: 15,
              pointRadius: 4,
              data: [80, 100, 70, 80, 120, 80],
            },
          ],
        },
        gradientColors: config.colors.primaryGradient,
        gradientStops: [1, 0.2, 0],
      },
      greenLineChart: {
        extraOptions: chartConfigs.greenChartOptions,
        chartData: {
          labels: ["JUL", "AUG", "SEP", "OCT", "NOV"],
          datasets: [
            {
              label: "My First dataset",
              fill: true,
              borderColor: config.colors.danger,
              borderWidth: 2,
              borderDash: [],
              borderDashOffset: 0.0,
              pointBackgroundColor: config.colors.danger,
              pointBorderColor: "rgba(255,255,255,0)",
              pointHoverBackgroundColor: config.colors.danger,
              pointBorderWidth: 20,
              pointHoverRadius: 4,
              pointHoverBorderWidth: 15,
              pointRadius: 4,
              data: [90, 27, 60, 12, 80],
            },
          ],
        },
        gradientColors: [
          "rgba(66,134,121,0.15)",
          "rgba(66,134,121,0.0)",
          "rgba(66,134,121,0)",
        ],
        gradientStops: [1, 0.4, 0],
      },
      blueBarChart: {
        extraOptions: chartConfigs.barChartOptions,
        chartData: {
          labels: ["USA", "GER", "AUS", "UK", "RO", "BR"],
          datasets: [
            {
              label: "Countries",
              fill: true,
              borderColor: config.colors.info,
              borderWidth: 2,
              borderDash: [],
              borderDashOffset: 0.0,
              data: [53, 20, 10, 80, 100, 45],
            },
          ],
        },
        gradientColors: config.colors.primaryGradient,
        gradientStops: [1, 0.4, 0],
      },
    };
  },
  computed: {
    enableRTL() {
      return this.$route.query.enableRTL;
    },
    isRTL() {
      return this.$rtl.isRTL;
    },
    bigLineChartCategories() {
      return this.$t("dashboard.chartCategories");
    },
  },
  methods: {
    initBigChart(index) {
      let chartData = {
        datasets: [
          {
            fill: true,
            borderColor: config.colors.primary,
            borderWidth: 2,
            borderDash: [],
            borderDashOffset: 0.0,
            pointBackgroundColor: config.colors.primary,
            pointBorderColor: "rgba(255,255,255,0)",
            pointHoverBackgroundColor: config.colors.primary,
            pointBorderWidth: 20,
            pointHoverRadius: 4,
            pointHoverBorderWidth: 15,
            pointRadius: 4,
            data: this.bigLineChart.allData[index],
          },
        ],
        labels: [
          "JAN",
          "FEB",
          "MAR",
          "APR",
          "MAY",
          "JUN",
          "JUL",
          "AUG",
          "SEP",
          "OCT",
          "NOV",
          "DEC",
        ],
      };
      this.$refs.bigChart.updateGradients(chartData);
      this.bigLineChart.chartData = chartData;
      this.bigLineChart.activeIndex = index;
    },
  },
  mounted() {
    this.i18n = this.$i18n;
    if (this.enableRTL) {
      this.i18n.locale = "ar";
      this.$rtl.enableRTL();
    }
    this.initBigChart(0);
  },
  beforeDestroy() {
    if (this.$rtl.isRTL) {
      this.i18n.locale = "en";
      this.$rtl.disableRTL();
    }
  },
};
</script>
<style></style>