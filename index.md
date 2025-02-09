---
layout: article
title: "XAI in Action: Past, Present, and Future Applications"
excerpt: NeurIPS 2023 Workshop
menu: true
show_info: true
titles:
  en      : &EN       Home
  en-GB   : *EN
  en-US   : *EN
  en-CA   : *EN
  en-AU   : *EN
key: page-home
article_header:
  type: overlay
  theme: dark
  align: left
  actions:
    - text: December 16, 2023 | New Orleans, USA 
  background_image:
    src: /assets/images/Slide6.png
#    gradient: 'linear-gradient(135deg, rgba(52, 140, 96, 0.4), rgba(136, 73, 107, 0.4))'
---

<style>
  
.schedule-table-heading {
    display: inline;
    font-weight: bold;
    font-size: 20px;
    color: #999999;
    padding:0 0 20px 0;
}

.schedule-table-timecol {
    padding:0 50px 0 50px;
    display:inline;
}

.schedule-table-eventcol {
    display:inline;
    display:inline-block;
    inline-size: 300px;
}

.schedule-table-contentcol {
    display:inline;
    display:inline-block;
    inline-size: 250px;
    font-size:14px;
    line-height: normal;
}

.schedule-table-row-even {
    display:block;
    width:800px;
    background-color: #EEEEEE;
    padding:10px;
}

.schedule-table-row-odd {
    display:block;
    width:800px;
    padding:10px;
}

.article__header--overlay .overlay {
    min-height: 36rem;
    padding-top: 5rem;
    padding-bottom: 5rem;
}

.article__header {
    margin: 0 0 0 0;
}

.article__header h1 {
    display: inline;
    font-family: sans-serif;
    font-size: 2.5em;
    letter-spacing: -0.04em;
    line-height: 0.9;
    color: lightyellow;
    text-shadow: -20px -8px 17px rgb(0 0 0 / 90%);
    -webkit-text-stroke: 2px black; /* width and color */
    word-wrap: break-word;
}

.overlay__excerpt {
    margin: 20px 0 0 0;
    font-family: sans-serif;
    color: black;
    text-shadow: -20px -8px 17px rgb(0 0 0 / 90%);
}

ul.menu li::after {
    color: black;
    text-shadow: -20px -8px 17px rgb(0 0 0 / 90%);
    content:"December 16, 2023 | New Orleans, USA";
}

ul.menu a {
    display: none;
}

.pc-column {
    width:270px;
    display:inline-block;
    vertical-align: top;
}

.pc_list_item {
    display:inline-block;
    width:200px;
}

.organiser_profile {
    font-weight:normal;
    color: black;
}

.organiser_profile a:link a:visited a:hover a:active {
    font-weight:normal;
    color: #000000;
}

.organiser_profile p {
    font-weight:normal;
    color: #000000;
}

.logos-organizers {
    display: flex;
    align-items: center;
    flex-direction: row;
    flex-wrap: nowrap;
}

.img-fluid {
    max-width: 100%;
    height: auto;
}

img {
    vertical-align: middle;
    border-style: none;
}





  


   body {
  font-family: 'Arial', sans-serif;
  line-height: 1.6;
  color: #333;
}

  .reviewers-container {
    display: flex;
    flex-wrap: wrap;
  }

  .reviewers-container > div {
    padding: 5px;
    background-color: #f0f0f0;
    border-radius: 5px;
    margin: 5px;
  }

  .sponsor-logos img {
    width: 150px; /* Adjust this value as needed */
    margin-right: 20px; /* Space between images */
}

/* Remove margin from the last image */
.sponsor-logos img:last-child {
    margin-right: 0;
}


  .toggle-button {
    background-color: #007bff; /* Blue background */
    color: white;
    padding: 10px 15px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    outline: none;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.toggle-button::after {
    content: ' ▼'; /* Down arrow by default */
}

.toggle-button.active::after {
    content: ' ▲'; /* Up arrow when the section is visible */
}


/* Optional: Style for paper titles */
.paper-title {
    font-weight: bold;
}

/* Optional: Style for authors */
.authors {
    font-style: italic;
}

table {
            width: 100%;
            border-collapse: collapse;
        }
        th, td {
            border: 1px solid black;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #f2f2f2;
        }

       .time {
            font-weight: bold;
            text-align: center;
        }
  
</style>


<script>

  
  var x = setInterval(function() {
    var d = new Date();
    var n = d.toLocaleTimeString("en-US", {timeZone: "America/New_York", hour: '2-digit', minute:'2-digit', hour12: false})
    document.getElementById("edt").innerHTML = n
  }, 1000);
</script>

<script>
  var x = setInterval(function() {
    var d = new Date();
    var n = d.toLocaleTimeString("en-US", {timeZone: "Europe/Vienna", hour: '2-digit', minute:'2-digit', hour12: false})
    document.getElementById("cet").innerHTML = n
  }, 1000);
</script>

<script>
  {%- include scripts/lib/swiper.js -%}
  var SOURCES = window.TEXT_VARIABLES.sources;
  window.Lazyload.js(SOURCES.jquery, function() {
    $('.swiper-demo').swiper();
  });
</script>

<script>

  var countDownDate = new Date("Feb 15, 2022 23:59:59 UTC").getTime();  
  countDownDate = countDownDate + 1000 * 3600 * 12


  var x = setInterval(function() {


    var now = new Date().getTime();


    var distance = countDownDate - now;


    var days = Math.floor(distance / (1000 * 60 * 60 * 24));
    var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
    var seconds = Math.floor((distance % (1000 * 60)) / 1000);


    var countdown = days + "d " + hours + "h " + minutes + "m " + seconds + "s ";


    if (distance < 0) {
      clearInterval(x);
      countdown = "(expired)";  
    }

    document.getElementById("countdown").innerHTML = countdown

  }, 1000);
</script>

<br>

## About

As AI models continue to advance in complexity and sophistication, understanding how they work and make decisions is becoming increasingly challenging. This challenge has prompted a surge of research into developing methods and tools that can enhance the transparency and explainability of these models. Nowadays, there are many such methods available, to the point that their specific applications have become somewhat unclear.

This workshop will specifically explore the diverse applications of explainable artificial intelligence (XAI) methods in various areas. The areas will include, but not limited to XAI in Healthcare, Natural Science, Auditing, Fairness, Natural Language Processing and Law. By examining the use of XAI in these fields, the workshop will provide attendees with insights into the latest trends and challenges within the different domains. 

The workshop discussions aim to delve into the latest advancements in applied XAI and devise ways to further progress the field. The objective is to foster an open and productive dialogue that enhances our understanding of the potential opportunities and constraints of XAI and its impact across different domains. The purpose of this discourse is to identify strategies that can extend the frontiers of applied XAI and make notable progress in this rapidly evolving area. Specifically, the workshop aims to:


### Topics covered

<div>
<div style="width:49%; display:inline-block; font-size:14px; vertical-align:top">
<ul>
<li>Examine various applications of XAI from the past and present </li>
<li>Discuss potential applications of XAI in the future</li>
<li>Identify the obstacles that hinder progress in each use case and how can we overcome them</li>
<li>Explore the necessary methodological requirements for applying XAI</li>
</ul>
</div>
<div style="width:49%; display:inline-block; font-size:14px; vertical-align:top">
<ul>
<li>Identify new domains where XAI can be useful in the future</li>
<li>Understand the inherent limitations of XAI</li>
<li>Explore whether insights gained from one use case can be transferred to other use cases</li>
</ul>
</div>
</div>

The workshop will provide a valuable learning opportunity for researchers, practitioners, and students seeking to apply XAI in their work, as it will feature presentations by experts in the field, as well as interactive discussions and insights into the latest trends and future directions in applied XAI. By bringing together a diverse group of participants with a shared interest in XAI, the workshop aims to foster collaboration, innovation, and knowledge sharing in this rapidly growing field.

## Accepted Papers

A full list of accepted papers can be found [here](https://openreview.net/group?id=NeurIPS.cc/2023/Workshop/XAIA&referrer=%5BHomepage%5D(%2F)#tab-accept).

### Oral Papers

<button id="toggle-oral-papers" class="toggle-button">Show Oral Papers</button>
<div id="oral-papers-list" class="reviewers-container" style="display: none;">
  <div><span class="paper-title">"Scale Alone Does not Improve Mechanistic Interpretability in Vision Models".</span> <span class="authors">Roland Zimmermann, Thomas Klein, Wieland Brendel.</span></div>
  <div><span class="paper-title">"Understanding Scalable Perovskite Solar Cell Manufacturing with Explainable AI".</span> <span class="authors">Lukas Klein, Sebastian Ziegler, Felix Laufer, Charlotte Debus, Markus Götz, Klaus Maier-Hein, Ulrich Paetzold, Fabian Isensee, Paul Jaeger.</span></div>
  <div><span class="paper-title">"Emergence of Segmentation with Minimalistic White-Box Transformers".</span> <span class="authors">Yaodong Yu, Tianzhe Chu, Shengbang Tong, Ziyang Wu, Druv Pai, Sam Buchanan, Yi Ma.</span></div>
  <div><span class="paper-title">"On Evaluating Explanation Utility for Human-AI Decision-Making in NLP".</span> <span class="authors">Fateme Hashemi Chaleshtori, Atreya Ghosal, Ana Marasovic.</span></div>
</div>

### Highlighted Reviewers

<button id="toggle-highlighted" class="toggle-button">Show Highlighted Reviewers</button>
<div id="highlighted-reviewers-list" class="reviewers-container" style="display: none;">
  <div>Sichao Li</div>
  <div>Bardh Prenkaj</div>
  <div>Arnaud Pannatier</div>
  <div>Kyle Matoba</div>
  <div>Amir Akbarnejad</div>
  <div>Nari Johnson</div>
  <div>Davin Hill</div>
  <div>Eike Peterson</div>
  <div>Karel D'Oosterlinck</div>
  <div>Bitya Neuhof</div>
  <div>Sebastian Bordt</div>
</div>

### All Reviewers

<button id="toggle-all" class="toggle-button">Show All Reviewers</button>
<div id="all-reviewers-list" class="reviewers-container dropdown-content" style="display: none;">
  <div>Sahib Singh</div>
  <div>Shah Nawaz</div>
  <div>Raj Korpan</div>
  <div>Zhenjie Zhao</div>
  <div>Sichao Li</div>
  <div>Eike Petersen</div>
  <div>Kiet Van Nguyen</div>
  <div>Rakshit Naidu</div>
  <div>Sukriti Verma</div>
  <div>Chris Lin</div>
  <div>Gabriel Kasmi</div>
  <div>Kilian Kluge</div>
  <div>Pulkit Verma</div>
  <div>Jacopo Teneggi</div>
  <div>Wei Qiu</div>
  <div>Muhammad Usman Shahid Khan</div>
  <div>Bardh Prenkaj</div>
  <div>Gökhan Özbulak</div>
  <div>Daniel Barrejon</div>
  <div>Fan Feng</div>
  <div>Hangzhi Guo</div>
  <div>Debarpan Bhattacharya</div>
  <div>Zeming Wei</div>
  <div>Sagnik Dakshit</div>
  <div>Arnav Wadhwa</div>
  <div>Beepul Bharti</div>
  <div>Sukrut Rao</div>
  <div>Pouya Khani</div>
  <div>Satyapriya Krishna</div>
  <div>Akshay R. Kulkarni</div>
  <div>Nitsan Soffair</div>
  <div>Bhawesh Kumar</div>
  <div>Yuri Feldman</div>
  <div>Lenka Tětková</div>
  <div>Wenbo Zhang</div>
  <div>Vinitra Swamy</div>
  <div>Sree Harsha Tanneru</div>
  <div>Daniel Flores Araiza</div>
  <div>Vidhya Kamakshi</div>
  <div>Goutham Rajendran</div>
  <div>Aditya Bhattacharya</div>
  <div>Swagatam Haldar</div>
  <div>Leonardo Lucio Custode</div>
  <div>Jaakko Suutala</div>
  <div>Changjian Shui</div>
  <div>Sasikanth Kotti</div>
  <div>Nan Wu</div>
  <div>Amir Akbarnejad</div>
  <div>Ido Ben-Shaul</div>
  <div>Kenza Amara</div>
  <div>Zeyu Qin</div>
  <div>Leonard Tang</div>
  <div>Raghav Singhal</div>
  <div>Mustafa Cavus</div>
  <div>Laura O'Mahony</div>
  <div>Canyu Chen</div>
  <div>Alex Oesterling</div>
  <div>Srishti Gautam</div>
  <div>Usha Bhalla</div>
  <div>Francesco Croce</div>
  <div>Alexander Meinke</div>
  <div>Christian Schlarmann</div>
  <div>Gal Yona</div>
  <div>Dana Arad</div>
  <div>Natalie Shapira</div>
  <div>Katelyn Morrison</div>
  <div>Maksym Andriushchenko</div>
  <div>Sunnie S. Y. Kim</div>
</div>

### Area Chairs

<button id="toggle-area-chairs" class="toggle-button">Show Area Chairs</button>
<div id="area-chairs-list" class="reviewers-container" style="display: none;">
  <div>Suraj Srinivas</div>
  <div>Valentyn Boreiko</div>
  <div>Chhavi Yadav</div>
  <div>Aounon Kumar</div>
  <div>Cyrus Rashtchian</div>
  <div>Michal Moshkovitz</div>
  <div>Nave Frost</div>
</div>


## Dates

Note: all deadlines are in <b>Anywhere on Earth (AoE)</b>.

### Paper Submission

Submission deadline - ~~September 22~~ October 2 (23:59 AoE), 2023 \
Author notification - ~~October 20~~ October 27 (23:59 AoE), 2023 \
Camera ready deadline -  November 22 (23:59 AoE), 2023

### Workshop Event

<b>Date:</b> December 16, 2023

## Schedule

<table>
    <tr>
        <th>Time</th>
        <th>Event</th>
        <th>Additional Information</th>
    </tr>
    <tr>
        <td class="time">8:50 - 9:00 AM</td>
        <td>Opening Remarks</td>
        <td></td>
    </tr>
    <tr>
        <td class="time">9:00 - 9:30 AM</td>
        <td>IT1: Sameer Singh</td>
        <td>
          <strong>Title:</strong> Explanations: Let's talk about them! <br>
          <button class="toggle-button" onclick="toggleAbstract('abstract_sameer')">Show Abstract</button>
            <div id="abstract_sameer" style="display:none;">
                Posthoc explanations aim to give end-users insights and understanding into the workings of complex machine learning models. Despite their potential, posthoc explanations have found limited use in real-world applications and, for some evaluation setups, fail to help end-users achieve their tasks effectively. In a survey we carried out with domain experts to understand why they do not use explanation techniques, they pointed out that explanations are static and inflexible, making it challenging to explore the model behavior intuitively. Based on these insights, we propose a shift towards natural language conversations as a promising avenue for future work for explainability: they are easy to use, flexible, and interactive. We introduce an initial version of such a system, TalkToModel, that uses LLMs to enable open-ended natural language conversations for machine learning explainability. In our evaluation, TalkToModel can accurately identify diverse user intents and support various user queries. Further, users strongly prefer TalkToModel over existing explainability systems, demonstrating the effectiveness of natural language interfaces in supporting model understanding. (This is work with Dylan Slack, Satya Krishna, Hima Lakkaraju, Chenhao Tan, and Yuxin Chen)
            </div>
        </td>
    </tr>
    <tr>
        <td class="time">9:30 - 10:00 AM</td>
        <td>IT2: Ulrike von Luxburg ※</td>
        <td>
          <strong>Title:</strong> Theoretical guarantees for explainable AI? <br>
            <button class="toggle-button" onclick="toggleAbstract('abstract_ulrike')">Show Abstract</button>
            <div id="abstract_ulrike" style="display:none;">
               Explainable machine learning is often discussed as a tool to
increase trust in machine learning systems. In my opinion,
this can only work if the explanations are trustworthy
themselves: we should be able to prove strong guarantees on
the explanations provided. In my presentation I will argue
that strong explanations in interesting scenarios might be
difficult to achieve.
            </div>
        </td>
    </tr>
    <tr>
        <td class="time">10:00 - 10:30 AM</td>
        <td>Coffee Break & Interactive Games</td>
        <td></td>
    </tr>
    <tr>
        <td class="time">10:30 - 11:00 AM</td>
        <td>IT3: Su-In Lee</td>
        <td><strong>Title:</strong> Explainable AI, where we are and how to move forward for health AI. </td>
    </tr>
    <tr>
        <td class="time">11:00 - 12:00 PM</td>
        <td>Panel Discussion</td>
        <td><strong>Moderator:</strong> Kamalika Chaudhuri. <br><strong>Panelists:</strong> Shai Ben-David, Julius Adebayo, Sameer Singh, Su-In Lee, Leilani Gilpin.</td>
    </tr>
    <tr>
        <td class="time">12:00 - 1:30 PM</td>
        <td>Lunch</td>
        <td></td>
    </tr>
    <tr>
        <td class="time">1:30 - 2:00 PM</td>
        <td>IT4: Julius Adebayo</td>
        <td>
            <strong>Title:</strong> Confronting the Faithfulness Challenge with Post-hoc Model Explanations. <br>
            <button class="toggle-button" onclick="toggleAbstract('abstract4')">Show Abstract</button>
            <div id="abstract4" style="display:none;">
                Explaining the output of a trained deep neural network has emerged as a key research challenge. Several classes of explanation methods (feature attributions, training point ranking, post-hoc concept attribution) have been proposed to address that challenge. However, despite significant research contributions, evidence points to their ineffectiveness.
In this talk, I'll highlight a key challenge that undercuts the effectiveness of current post hoc explanations methods: <i>faithfulness</i>. A model's explanation is faithful if the feature importance score, induced by the explanation, indicates the magnitude of the change in the model's output, when that feature is ablated. However, consistent evidence indicates that post hoc explanations of large-scale deep nets, under standard training regimes, are unfaithful. I'll close with two vignettes: the first on emerging recipes for overcoming the faithfulness challenge, and the second on an alternative paradigm that involves developing intrinsically interpretable models.
            </div>
        </td>
    </tr>
    <tr>
        <td class="time">2:00 - 3:00 PM</td>
        <td>Poster Session 1</td>
        <td>
          <button class="toggle-button" onclick="togglePapers('papers1')">Show Papers</button>
          <div id="papers1" class="papers-container" style="display:none;">
            <div>Paper ID: 1 - <a href="https://openreview.net/forum?id=gh69Bu7k48">"Geometric Remove-and-Retrain (GOAR): Coordinate-Invariant eXplainable AI Assessment"</a></div>
            <div>Paper ID: 2 - <a href="https://openreview.net/forum?id=iqXixXrMKa">"How Well Do Feature-Additive Explainers Explain Feature-Additive Predictors?"</a></div>
            <div>Paper ID: 4 - <a href="https://openreview.net/forum?id=WyBAWwpqTY">"Scale Alone Does not Improve Mechanistic Interpretability in Vision Models"</a></div>
            <div>Paper ID: 5 <b>(DEMO)</b> - <a href="https://openreview.net/forum?id=fPnpjEhyxv">"Utilizing Explainability Techniques for Reinforcement Learning Model Assurance"</a></div>
            <div>Paper ID: 8 - <a href="https://openreview.net/forum?id=w6Qnoy2RXG">"GInX-Eval: Towards In-Distribution Evaluation of Graph Neural Network Explanations"</a></div>
            <div>Paper ID: 9 - <a href="https://openreview.net/forum?id=d7FsEtYjvN">"Towards the next generation explainable AI that promotes AI-human mutual understanding"</a></div>
            <div>Paper ID: 10 - <a href="https://openreview.net/forum?id=112o4j4VCY">"Assessment of the Reliablity of a Model's Decision by Generalizing Attribution to the Wavelet Domain"</a></div>
            <div>Paper ID: 11 - <a href="https://openreview.net/forum?id=3oysFpd6Pq">"Influence Based Approaches to Algorithmic Fairness: A Closer Look"</a></div>
            <div>Paper ID: 12 <b>(DEMO)</b> - <a href="https://openreview.net/forum?id=81FSrQxgEv">"ExpLIMEable: An exploratory framework for LIME"</a></div>
            <div>Paper ID: 13 - <a href="https://openreview.net/forum?id=xrEpp63kz7">"Understanding Scalable Perovskite Solar Cell Manufacturing with Explainable AI"</a></div>
            <div>Paper ID: 14 - <a href="https://openreview.net/forum?id=ewagDhIy8Y">"Detecting Spurious Correlations via Robust Visual Concepts in Real and AI-Generated Image Classification"</a></div>
            <div>Paper ID: 16 - <a href="https://openreview.net/forum?id=3BX9tM03GT">"Explaining black box text modules in natural language with language models"</a></div>
            <div>Paper ID: 18 - <a href="https://openreview.net/forum?id=lERHoohuX5">"Lessons from Usable ML Deployments and Application to Wind Turbine Monitoring"</a></div>
            <div>Paper ID: 21 - <a href="https://openreview.net/forum?id=FSmlu6xrUt">"Beyond Concept Bottleneck Models: How to Make Black Boxes Intervenable?"</a></div>
            <div>Paper ID: 24 - <a href="https://openreview.net/forum?id=yCQC8hLyZj">"Emergence of Segmentation with Minimalistic White-Box Transformers"</a></div>
            <div>Paper ID: 25 - <a href="https://openreview.net/forum?id=CKPGhnMADQ">"Optimising Human-AI Collaboration by Learning Convincing Explanations"</a></div>
            <div>Paper ID: 26 - <a href="https://openreview.net/forum?id=9i4AcMYE6o">"Inherent Inconsistencies of Feature Importance"</a></div>
            <div>Paper ID: 27 - <a href="https://openreview.net/forum?id=2CfzKrx1vr">"Use Perturbations when Learning from Explanations"</a></div>
            <div>Paper ID: 28 - <a href="https://openreview.net/forum?id=DkyNNQPmSj">"Estimation of Concept Explanations Should be Uncertainty Aware"</a></div>
            <div>Paper ID: 29 - <a href="https://openreview.net/forum?id=bhvlGMbONN">"Are VideoQA Models Truly Multimodal?"</a></div>
            <div>Paper ID: 30 - <a href="https://openreview.net/forum?id=cBXiaGUcK8">"Extracting human interpretable structure-property relationships in chemistry using XAI and large language models"</a></div>
            <div>Paper ID: 31 - <a href="https://openreview.net/forum?id=nVGuWh4S2G">"Towards Explanatory Model Monitoring"</a></div>
            <div>Paper ID: 32 - <a href="https://openreview.net/forum?id=hkfsR3HMuj">"Diagnosing Transformers: Illuminating Feature Spaces for Clinical Decision-Making"</a></div>
            <div>Paper ID: 33 - <a href="https://openreview.net/forum?id=se4ojQqjB5">"Explainable AI in Music Performance: Case Studies from Live Coding and Sound Spatialisation"</a></div>
            <div>Paper ID: 34 - <a href="https://openreview.net/forum?id=YVQSGT6ME0">"COMET: Neural Cost Model Explanation Framework"</a></div>
            <div>Paper ID: 35 - <a href="https://openreview.net/forum?id=Zbt9z0a95l">"Piecewise Linear Parametrization of Policies: Towards Interpretable Deep Reinforcement Learning"</a></div>
            <div>Paper ID: 36 <b>(DEMO)</b> - <a href="https://openreview.net/forum?id=jnNixRhhF8">"DeepDecipher: Accessing and Investigating Neuron Activation in Large Language Models"</a></div>
            <div>Paper ID: 37 <b>(DEMO)</b> - <a href="https://openreview.net/forum?id=JqfN8vp1ov">"Interactive Visual Feature Search"</a></div>
            <div>Paper ID: 40 - <a href="https://openreview.net/forum?id=h5usKrxCH2">"AttributionLab: Faithfulness of Feature Attribution Under Controllable Environments"</a></div>
            <div>Paper ID: 42 - <a href="https://openreview.net/forum?id=uU1eXPwesa">"FRUNI and FTREE synthetic knowledge graphs for evaluating explainability"</a></div>
        </div>
        </td>
    </tr>
    <tr>
        <td class="time">3:00 - 3:30 PM</td>
        <td>Coffee Break & Interactive Games</td>
        <td>
        </td>
    </tr>
    <tr>
        <td class="time">3:30 - 4:00 PM</td>
        <td>IT5: Leilani Gilpin</td>
        <td>
            <strong>Title:</strong> Explaining Self-Driving Cars for Accountable Autonomy. <br>
            <button class="toggle-button" onclick="toggleAbstract('abstract5')">Show Abstract</button>
            <div id="abstract5" style="display:none;">
                Autonomous systems are prone to errors and failures without knowing
why. In critical domains like driving, these autonomous counterparts
must be able to recount their actions for safety, accountability, and
trust. An explanation: a model-dependent reason or justification for
the decision of the autonomous agent being assessed, is a key
component for post-mortem failure analysis, but also for
pre-deployment verification. I will present neuro-symbolic systems
that use neural networks and commonsense knowledge to detect and
explain unreasonable vehicle scenarios, even if the autonomous vehicle
has not seen that error before. In the second part of the talk, I will
motivate the use of explanations as a testing framework for autonomous
systems. I will conclude by discussing new challenges at the
intersection of explainable AI and autonomy toward autonomous vehicles
systems that are explainable by design.
            </div>
        </td>
    </tr>
    <tr>
        <td class="time">4:00 - 4:30 PM</td>
        <td>Contributed Talks</td>
        <td></td>
    </tr>
    <tr>
        <td class="time">4:30 - 5:30 PM</td>
        <td>Poster Session 2</td>
        <td>
        <button class="toggle-button" onclick="togglePapers('papers2')">Show Papers</button>
        <div id="papers2" class="papers-container" style="display:none;">
            <div>Paper ID: 44 - <a href="https://openreview.net/forum?id=9yXEqVKacK">"GLANCE: Global to Local Architecture-Neutral Concept-based Explanations"</a></div>
            <div>Paper ID: 45 - <a href="https://openreview.net/forum?id=ThwzmgEwm5">"ReLax: An Efficient and Scalable Recourse Explanation Benchmarking Library using JAX"</a></div>
            <div>Paper ID: 46 - <a href="https://openreview.net/forum?id=SCcOu4hJ97">"Caution to the Exemplars: On the Intriguing Effects of Example Choice on Human Trust in XAI"</a></div>
            <div>Paper ID: 47 - <a href="https://openreview.net/forum?id=iMR4ukkUFU">"A Simple Scoring Function to Fool SHAP: Stealing from the One Above"</a></div>
            <div>Paper ID: 48 <b>(DEMO)</b> - <a href="https://openreview.net/forum?id=r1CV7mhvdS">"Transparent Anomaly Detection via Concept-based Explanations"</a></div>
            <div>Paper ID: 49 - <a href="https://openreview.net/forum?id=KPtW2SU0my">"The Disagreement Problem in Faithfulness Metrics"</a></div>
            <div>Paper ID: 50 - <a href="https://openreview.net/forum?id=ANrzX5KFAG">"Diffusion-Guided Counterfactual Generation for Model Explainability"</a></div>
            <div>Paper ID: 52 - <a href="https://openreview.net/forum?id=x9H6lNez5b">"Exploring Practitioner Perspectives On Training Data Attribution Explanations"</a></div>
            <div>Paper ID: 53 - <a href="https://openreview.net/forum?id=8BR8EaWNTZ">"On Evaluating Explanation Utility for Human-AI Decision-Making in NLP"</a></div>
            <div>Paper ID: 54 <b>(DEMO)</b> - <a href="https://openreview.net/forum?id=GL7RDOru1k">"Empowering Domain Experts to Detect Social Bias in Generative AI with User-Friendly Interfaces"</a></div>
            <div>Paper ID: 55 - <a href="https://openreview.net/forum?id=xuT2SDuJX6">"A Critical Survey on Fairness Benefits of XAI"</a></div>
            <div>Paper ID: 56 - <a href="https://openreview.net/forum?id=uVAiiHFH0L">"Stability Guarantees for Feature Attributions with Multiplicative Smoothing"</a></div>
            <div>Paper ID: 57 - <a href="https://openreview.net/forum?id=tiLZkab8TP">"On the Consistency of GNN Explainability Methods"</a></div>
            <div>Paper ID: 59 - <a href="https://openreview.net/forum?id=OIbmpF4ZR9">"Explaining Tree Model Decisions in Natural Language for Network Intrusion Detection"</a></div>
            <div>Paper ID: 63 - <a href="https://openreview.net/forum?id=F6RPYDUIZr">"Do Concept Bottleneck Models Obey Locality?"</a></div>
            <div>Paper ID: 64 - <a href="https://openreview.net/forum?id=vVpefYmnsG">"Sanity Checks Revisited: An Exploration to Repair the Model Parameter Randomisation Test"</a></div>
            <div>Paper ID: 68 - <a href="https://openreview.net/forum?id=h6OT5pzrGc">"Visual Topics via Visual Vocabularies"</a></div>
            <div>Paper ID: 70 - <a href="https://openreview.net/forum?id=joaWGug1CU">"Explainable Reinforcement Learning for Alzheimer’s Disease Progression Prediction."</a></div>
            <div>Paper ID: 71 - <a href="https://openreview.net/forum?id=wNhcShUyAf">"Explaining high-dimensional text classifiers"</a></div>
            <div>Paper ID: 72 - <a href="https://openreview.net/forum?id=wFJoNkiASU">"Sum-of-Parts Models: Faithful Attributions for Groups of Features"</a></div>
            <div>Paper ID: 74 - <a href="https://openreview.net/forum?id=hpuOA3nkVW">"Explaining Longitudinal Clinical Outcomes using Domain-Knowledge driven Intermediate Concepts"</a></div>
            <div>Paper ID: 75 - <a href="https://openreview.net/forum?id=lJ63ABWs8V">"Rectifying Group Irregularities in Explanations for Distribution Shift"</a></div>
            <div>Paper ID: 76 - <a href="https://openreview.net/forum?id=mAzhEP9jPv">"Are Large Language Models Post Hoc Explainers?"</a></div>
            <div>Paper ID: 78 - <a href="https://openreview.net/forum?id=N5RmOXuTDo">"ObEy: Quantifiable Object-based Explainability without Ground-Truth Annotations"</a></div>
            <div>Paper ID: 79 - <a href="https://openreview.net/forum?id=Liw9vOCxe2">"Cost-aware counterfactuals for black box explanations"</a></div>
            <div>Paper ID: 83 - <a href="https://openreview.net/forum?id=qt9yTS7TKc">"Robust Recourse for Binary Allocation Problems"</a></div>
            <div>Paper ID: 84 <b>(DEMO)</b> - <a href="https://openreview.net/forum?id=QPqL9xsYOf">"Policy graphs in action: explaining single- and multi-agent behaviour using predicates"</a></div>
            <div>Paper ID: 85 - <a href="https://openreview.net/forum?id=ag1CpSUjPS">"On the Relationship Between Explanation and Prediction: A Causal View"</a></div>
            <div>Paper ID: 86 - <a href="https://openreview.net/forum?id=bGsW1wSIxQ">"Interactive Model Correction with Natural Language"</a></div>
        </div>
        </td>

    </tr>
</table>

※ Indicates virtual participation

_All times are in Central Standard Time_  

<!---
Friday, 22 July, 2022. All times are in Eastern Daylight Time (EDT). Current time is <span id="edt"></span>.

<div style="display:block; width:900px; padding:20px; border:solid 4px #CCCCCC;">
<div class="schedule-table-heading" style="margin-left:57px; display:inline-block; inline-size:100px;">Time</div>
<div class="schedule-table-heading" style="display:inline-block; inline-size:295px;">Event</div>
<div class="schedule-table-heading">Content</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">08:50</div>
<div class="schedule-table-eventcol">Welcome</div>
<div class="schedule-table-contentcol">Opening Remarks</div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">09:00</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/david_held.png" alt="David Held">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">David Held</p>
<p style="margin:0 0 0 10px; font-size:10px;">CMU</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987747/selfsupervised-3d-perception-for-autonomous-driving?ref=folder-105306" target="_blank"><i>Self-supervised learning for autonomous driving</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">09:30</div>
<div class="schedule-table-eventcol">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/melanie_zeilinger.png" alt="Melanie Zeilinger">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Melanie Zeilinger</p>
<p style="margin:0 0 0 10px; font-size:10px;">ETH Zürich</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987741/learning-for-high-performance-yet-safe-control?ref=folder-105306"><i>Learning for High Performance yet Safe Control</i></a></div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol">10:00</div>
<div class="schedule-table-eventcol">Social + Poster Session</div>

<div class="schedule-table-contentcol"><b>Gathertown</b> and in-person displays</div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">11:00</div>
<div class="schedule-table-eventcol">Spotlight Talks</div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">&nbsp;</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
&nbsp;
</div>
<div style="display:inline-block; width:150px; line-height:1.4; margin:0 0 0 40px">
<p style="margin:0 0 0 10px;">Zijian Guo</p>
<p style="margin:0 0 0 10px; font-size:10px;">CMU</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol" style="margin:0 0 0 35px;"><a target="_blank" href="https://slideslive.com/38987752/constrained-modelbased-reinforcement-learning-via-robust-planning?ref=folder-105306"><i>#16: Constrained Model-based Reinforcement Learning via Robust Planning</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">&nbsp;</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
&nbsp;
</div>
<div style="display:inline-block; width:150px; line-height:1.4; margin:0 0 0 40px">
<p style="margin:0 0 0 10px;">Linrui Zhang</p>
<p style="margin:0 0 0 10px; font-size:10px;">Tsinghua University</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol" style="margin:0 0 0 35px;"><a target="_blank" href="https://slideslive.com/38987764/saferlkit-evaluating-efficient-reinforcement-learning-methods-for-safe-autonomous-driving?ref=folder-105306"><i>#12: SafeRL-Kit: Evaluating Efficient Reinforcement Learning Methods for Safe Autonomous Driving</i></a></div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">11:30</div>
<div class="schedule-table-eventcol">Autonomous Racing Virtual Challenge: Contributed Talks</div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">&nbsp;</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
&nbsp;
</div>
<div style="display:inline-block; width:150px; line-height:1.4; margin:0 0 0 40px">
<p style="margin:0 0 0 10px;">Shivansh Beohar</p>
<p style="margin:0 0 0 10px; font-size:10px;">IIIT Allahabad</p>
</div>
</div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">&nbsp;</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
&nbsp;
</div>
<div style="display:inline-block; width:150px; line-height:1.4; margin:0 0 0 40px">
<p style="margin:0 0 0 10px;">James Bockman</p>
<p style="margin:0 0 0 10px; font-size:10px;">U Adelaide</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol" style="margin:0 0 0 35px;"><a target="_blank" href="https://slideslive.com/38987768/the-edge-of-disaster-a-battle-between-autonomous-racing-and-safety?ref=folder-105306"><i>#14: The Edge of Disaster: A Battle Between Autonomous Racing and Safety</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">12:00</div>
<div class="schedule-table-eventcol">Lunch Break</div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">13:30</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/peter_stone.png" alt="Peter Stone">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Peter Stone</p>
<p style="margin:0 0 0 10px; font-size:10px;">UT Austin; Sony AI</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987742/reward-misdesign-for-autonomous-driving-and-accumulating-safety-rules-from-catastrophic-action-effects?ref=folder-105306"><i>Reward (Mis)design for Autonomous Driving and Accumulating Safety Rules from Catastrophic Action Effects</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">14:00</div>
<div class="schedule-table-eventcol">Spotlight Talks</div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">&nbsp;</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
&nbsp;
</div>
<div style="display:inline-block; width:150px; line-height:1.4; margin:0 0 0 40px">
<p style="margin:0 0 0 10px;">Weiran Yao</p>
<p style="margin:0 0 0 10px; font-size:10px;">CMU</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol" style="margin:0 0 0 35px;"><a target="_blank" href="https://slideslive.com/38987757/distributionaware-goal-prediction-and-conformant-modelbased-planning-for-safe-autonomous-driving?ref=folder-105306"><i>#23: Distribution-aware Goal Prediction and Conformant Model-based Planning for Safe Autonomous Driving</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">&nbsp;</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
&nbsp;
</div>
<div style="display:inline-block; width:150px; line-height:1.4; margin:0 0 0 40px">
<p style="margin:0 0 0 10px;">Zuxin Liu</p>
<p style="margin:0 0 0 10px; font-size:10px;">CMU</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol" style="margin:0 0 0 35px;"><a target="_blank" href="https://slideslive.com/38987751/on-the-robustness-of-safe-reinforcement-learning-under-observational-perturbations?ref=folder-105306"><i>#15: On the Robustness of Safe Reinforcement Learning under Observational Perturbations</i></a></div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">14:30</div>
<div class="schedule-table-eventcol">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/todd_hester.png" alt="Todd Hester">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Todd Hester</p>
<p style="margin:0 0 0 10px; font-size:10px;">Amazon Scout</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987743/multimodal-sensor-fusion-for-the-amazon-scout-robot?ref=folder-105306"><i>Multi-modal sensor fusion for the Amazon Scout robot</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">15:00</div>
<div class="schedule-table-eventcol">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/chelsea_finn.png" alt="Chelsea Finn">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Chelsea Finn</p>
<p style="margin:0 0 0 10px; font-size:10px;">Stanford + Google Brain</p>
</div>
</div>
</div>


<div class="schedule-table-row-odd">
<div class="schedule-table-timecol">15:30</div>
<div class="schedule-table-eventcol">Social + Poster Session</div>

<div class="schedule-table-contentcol"><b>Gathertown</b> and in-person displays</div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">16:30</div>
<div class="schedule-table-eventcol">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/andrea_bajcsy.png" alt="Andrea Bajcsy">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Andrea Bajcsy</p>
<p style="margin:0 0 0 10px; font-size:10px;">UC Berkeley / CMU</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987745/practical-safety-assurances-for-dynamic-humanrobot-interactions?ref=folder-105306"><i>Practical Safety Assurances for Dynamic Human-Robot Interactions</i></a></div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">17:00</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/jeff_schneider.png" alt="Jeff Schneider">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Jeff Schneider</p>
<p style="margin:0 0 0 10px; font-size:10px;">Carnegie Mellon University</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987746/safety-and-reinforcement-learning-for-selfdriving-cars?ref=folder-105306"><i>Reinforcement Learning for self-driving cars</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">17:30</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/sergey_levine.png" alt="Sergey Levine">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Sergey Levine</p>
<p style="margin:0 0 0 10px; font-size:10px;">UC Berkeley</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987748/learning-plannable-representations-and-planning-with-learnable-skills?ref=folder-105306"><i>Learning Plannable Representations and Planning with Learnable Skills</i></a></div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol">18:00</div>
<div class="schedule-table-eventcol">Conclusion</div>
<div class="schedule-table-contentcol">Closing Remarks</div>
</div>

</div>

--->

## Speakers


<div style="display:inline; width:900px; vertical-align: top;">

<a href="https://juliusadebayo.com/" target="_blank" class="speaker_profile">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/speakers/AXAI_workshop_julius.png" alt="Julius Adebayo">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Julius Adebayo</p>
<p style="margin:0 0 0 10px; font-size:10px;">Postdoctoral Fellow<br>Prescient Design</p>
</div>
</div>
</a>




<a href="https://people.ucsc.edu/~lgilpin/" target="_blank" class="speaker_profile">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/speakers/AXAI_workshop_leilani.png" alt="Leilani Gilpin">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Leilani Gilpin</p>
<p style="margin:0 0 0 10px; font-size:10px;">Assistant Professor<br>UC Santa Cruz</p>
</div>
</div>
</a>

<a href="https://aims.cs.washington.edu/su-in-lee" target="_blank" class="speaker_profile">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="/assets/images/speakers/AXAI_workshop_Lee.png" alt="Su-In Lee" />
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Su-In Lee</p>
<p style="margin:0 0 0 10px; font-size:10px;">Professor<br />Paul G. Allen School of Computer Science & Engineering</p>
</div>
</div>
</a>

<a href="https://www.tml.cs.uni-tuebingen.de/team/luxburg/" target="_blank" class="speaker_profile">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/speakers/AXAI_workshop_ulrike.png" alt="Ulrike von Luxburg">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Ulrike von Luxburg</p>
<p style="margin:0 0 0 10px; font-size:10px;">Professor<br>University of Tübingen </p>
</div>
</div>
</a>


<a href="https://sameersingh.org/" target="_blank" class="speaker_profile">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/speakers/AXAI_workshop_sameer.png" alt="Sameer Singh">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Sameer Singh</p>
<p style="margin:0 0 0 10px; font-size:10px;">Associate Professor<br>University of California, Irvine</p>
</div>
</div>
</a>



</div>


## Organisers


<div style="display:inline; width:900px; vertical-align: top;">

<a href="https://www.chhaviyadav.org" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/AXAI_workshop_chhavi.png" alt="Chhavi Yadav">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Chhavi Yadav</p>
<p style="margin:0 0 0 10px; font-size:10px;">PhD student at UCSD, her interests lie in XAI, Secure Verification, Auditing and societal impacts of deep generative models</p>
</div>
</div>
</a>

<a href="https://sites.google.com/view/michal-moshkovitz" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/AXAI_workshop_michal.png" alt="Michal Moshkovitz">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Michal Moshkovitz </p>
<p style="margin:0 0 0 10px; font-size:10px;">Machine Learning Research Scientist at Bosch Research, she has been focused on developing the foundations of explainable machine learning</p>
</div>
</div>
</a>

<a href="https://www.linkedin.com/in/bingqing-chen-631b754a/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/bingqing_chen.png" alt="Bingqing Chen">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Bingqing Chen</p>
<p style="margin:0 0 0 10px; font-size:10px;">Machine Learning Research Scientist at Bosch Research, her research lies at the intersection of machine learning and energy systems</p>
</div>
</div>
</a>

<a href="https://www.linkedin.com/in/nave-frost/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/AXAI_workshop_nave.png" alt="Nave Frost">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Nave Frost</p>
<p style="margin:0 0 0 10px; font-size:10px;">Research Scientist at eBay Research, his research interests focus on supplying explanations for data science applications</p>
</div>
</div>
</a>

<a href="https://suraj-srinivas.github.io" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/AXAI_workshop_suraj.png" alt="Suraj Srinivas">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Suraj Srinivas</p>
<p style="margin:0 0 0 10px; font-size:10px;">Postdoctoral research fellow at Harvard University, his research focuses on developing the foundations for interpretable machine learning</p>
</div>
</div>
</a>

<a href="https://scholar.google.com/citations?user=gzRuY4cAAAAJ&hl=en" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/AXAI_workshop_valentyn.png" alt="Valentyn Boreiko">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Valentyn Boreiko</p>
<p style="margin:0 0 0 10px; font-size:10px;">PhD student at the University of Tübingen and a sabbatical student at Bosch Research, his research focuses on development of interpretability technique for vision classifiers</p>
</div>
</div>
</a>

<a href="https://himalakkaraju.github.io" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/AXAI_workshop_hima.png" alt="Hima Lakkaraju">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Hima Lakkaraju</p>
<p style="margin:0 0 0 10px; font-size:10px;">Assistant Professor at Harvard University who focuses on the algorithmic and applied aspects of explainability, fairness, robustness, and privacy of machine learning models</p>
</div>
</div>
</a>


<a href="http://zicokolter.com" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/AXAI_workshop_zico.png" alt="Zico Kolter">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Zico Kolter</p>
<p style="margin:0 0 0 10px; font-size:10px;">Aassociate Professor at CMU, and chief scientist at Bosch Research, his work spans the intersection of machine learning and optimization</p>
</div>
</div>
</a>

<a href="https://scholar.google.co.il/citations?user=zhQaFaMAAAAJ&hl=en" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/AXAI_workshop_dotan.png" alt="Dotan Di Castro">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Dotan Di Castro</p>
<p style="margin:0 0 0 10px; font-size:10px;">Research scientist and lab manager at Bosch Research, his research focuses on Reinforcement Learning and Computer Vision</p>
</div>
</div>
</a>

<a href="https://cseweb.ucsd.edu/~kamalika/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/AXAI_workshop_kamalika.png" alt="Kamalika Chaudhuri">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Kamalika Chaudhuri</p>
<p style="margin:0 0 0 10px; font-size:10px;">Associate Professor at UCSD and a Research Scientist at Meta AI, her research interests lie in the foundations of trustworthy machine learning</p>
</div>
</div>
</a>

</div>


# Contact information

- Email: appliedXAI.neurips2023 [AT] gmail.com
- Twitter: [@XAI_in_Action](https://twitter.com/XAI_in_Action)


## Sponsors

<div class="sponsor-logos">
    <img src="{{ site.baseurl }}/assets/images/sponsors/bosch_logo.png" alt="Bosch Logo">
    <img src="{{ site.baseurl }}/assets/images/sponsors/Google_2015_logo.svg.png" alt="Google Logo">
</div>

<script>
 document.addEventListener('DOMContentLoaded', function() {

   // Toggle for Oral Papers
    var toggleHighlighted = document.getElementById('toggle-oral-papers');
    toggleHighlighted.addEventListener('click', function() {
        var div = document.getElementById('oral-papers-list');
        var isVisible = div.style.display === 'block';
        div.style.display = isVisible ? 'none' : 'block';
        toggleHighlighted.classList.toggle('active', !isVisible);
    });

   
    // Toggle for Highlighted Reviewers
    var toggleHighlighted = document.getElementById('toggle-highlighted');
    toggleHighlighted.addEventListener('click', function() {
        var div = document.getElementById('highlighted-reviewers-list');
        var isVisible = div.style.display === 'block';
        div.style.display = isVisible ? 'none' : 'block';
        toggleHighlighted.classList.toggle('active', !isVisible);
    });

    // Toggle for All Reviewers
    var toggleAll = document.getElementById('toggle-all');
    toggleAll.addEventListener('click', function() {
        var div = document.getElementById('all-reviewers-list');
        var isVisible = div.style.display === 'block';
        div.style.display = isVisible ? 'none' : 'block';
        toggleAll.classList.toggle('active', !isVisible);
    });

    // Toggle for Area Chairs
    var toggleAreaChairs = document.getElementById('toggle-area-chairs');
    toggleAreaChairs.addEventListener('click', function() {
        var div = document.getElementById('area-chairs-list');
        var isVisible = div.style.display === 'block';
        div.style.display = isVisible ? 'none' : 'block';
        toggleAreaChairs.classList.toggle('active', !isVisible);
    });
});


  function toggleAbstract(abstractId) {
        var abstract = document.getElementById(abstractId);
        if (abstract.style.display === "none") {
            abstract.style.display = "block";
        } else {
            abstract.style.display = "none";
        }
    }

  function togglePapers(papersId) {
    var papersDiv = document.getElementById(papersId);
    papersDiv.style.display = (papersDiv.style.display === "none") ? "block" : "none";
}
</script>
