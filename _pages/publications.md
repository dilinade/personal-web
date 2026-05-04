---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
classes: wide
---

### Conference and Workshop Papers
{: style="font-size:.85em; color: #7a8288;"}
---

<div class="section">
  <div class="section-item">
    <p class="p-no-margin-bottom"><strong><span class="new-prefix">(New)</span> Spandana: Reconciling Strict SLOs with Low Cost under Fine-Grained Load Fluctuations</strong><br>
    <u>D. Dehigama</u>, S. Jesalpura, Z. Xu, M. Nemeth, M. Kogias, and B. Grot<br>
    <span class="accepted-note">Accepted at <a href="https://acmsocc.org/2026/" target="_blank">ACM Symposium on Cloud Computing (SoCC), 2026</a></span></p>
    <div class="button-group">
      <a href="#" class="btn btn--primary btn-disabled" aria-disabled="true">Coming soon!</a>
      <button type="button" class="btn btn--primary bibtex-copy" data-bibtex-target="bibtex-spandana">Copy BibTeX</button>
    </div>
  </div>

  <div class="section-item">
    <p class="p-no-margin-bottom"><strong>Harmonizing Diverse Compute Resources for Efficiency</strong><br>
    <u>D. Dehigama</u>, S. Jesalpura, M. Kogias, and B. Grot<br>
    <em><a href="https://hotinfra24.github.io/" target="_blank">HotInfra Workshop at SOSP, 2024 (Austin, Texas)</a></em></p>
    <div class="button-group">
      <a href="https://www.research.ed.ac.uk/en/publications/harmonizing-diverse-compute-resources-for-efficiency/" target="_blank" class="btn btn--primary">Paper</a>
      <button type="button" class="btn btn--primary bibtex-copy" data-bibtex-target="bibtex-hotinfra">BibTeX</button>
    </div>
  </div>

  <div class="section-item">
    <p class="p-no-margin-bottom"><strong>Composing Microservices and Serverless for Load Resilience</strong><br>
    <u>D. Dehigama</u>, S. Jesalpura, A. Katsarakis, M. Kogias, R. Kumar, and B. Grot<br>
    <em><a href="https://sesame2024.github.io/" target="_blank">SESAME at EuroSys '24 (Athens, Greece)</a></em></p>
    <div class="button-group">
      <a href="https://www.research.ed.ac.uk/en/publications/composing-microservices-and-serverless-for-load-resilience/" target="_blank" class="btn btn--primary">Paper</a>
      <button type="button" class="btn btn--primary bibtex-copy" data-bibtex-target="bibtex-sesame">BibTeX</button>
    </div>
  </div>
</div>

<pre id="bibtex-spandana" class="bibtex-source" hidden>@inproceedings{dehigama2026spandana,
  title     = {Spandana: Reconciling Strict SLOs with Low Cost under Fine-Grained Load Fluctuations},
  author    = {Dehigama, Dilina and Jesalpura, Smit and Xu, Zhihao and Nemeth, Marcell and Kogias, Marios and Grot, Boris},
  booktitle = {Proceedings of the ACM Symposium on Cloud Computing (SoCC)},
  year      = {2026},
  note      = {Accepted}
}</pre>

<pre id="bibtex-hotinfra" class="bibtex-source" hidden>@inproceedings{d494de1d227b46ed8429240dd9f9625b,
title = "Harmonizing diverse compute resources for efficiency",
abstract = "Online services are characterized by significant load fluctuations at fine-grained intervals even when coarse-grained load measurements indicate a relatively stable load. Running such services on virtual machines (VMs) rented from a cloud provider like AWS, which is a typical way to deploy online applications today, is inefficient due to the need to overprovision VM capacity to meet the SLO under variable load. In contrast, serverless computing is highly elastic but is prohibitively expensive for serving a large volume of requests. We thus argue for combining the different types of compute (i.e., VM and serverless instances) to achieve both cost-efficiency and elasticity. Our results show that hybrid compute is more cost effective than even an optimal VMonly allocation that provisions just enough resource to meet the SLO using perfect knowledge of future load.",
author = "Dilina Dehigama and Shyam Jesalpura and Marios Kogias and Boris Grot",
year = "2024",
month = nov,
day = "3",
language = "English",
pages = "1--4",
booktitle = "Proceedings of the 2nd Workshop on Hot Topics in System Infrastructure",
publisher = "Association for Computing Machinery (ACM)",
address = "United States",
note = "The 2nd Workshop on Hot Topics in System Infrastructure, HotInfra'24 ; Conference date: 03-11-2024 Through 03-11-2024",
url = "https://hotinfra24.github.io/",
}</pre>

<pre id="bibtex-sesame" class="bibtex-source" hidden>@conference{9987358b722b4062a1ace674d6699335,
title = "Composing microservices and serverless for load resilience",
abstract = "Online services strive to maintain application responsiveness even when the traffic is unpredictable and fluctuating. Today{\textquoteright}s online services are commonly deployed as graphs of microservices, each microservice packaged as one or more containers inside a virtual machines (VMs). While performant and affordable when the load is steady, VM-based deployments are known to be slow to scale when the load spikes, resulting in degraded performance for end-users of the service. To avoid such performance degradations, service providers can over-provision their deployments; however, such a strategy is costly and inefficient, leaving resources heavily under-utilized for extended periods of time. To address this challenge, we propose Hydra, a hybrid architecture that combines microservices with serverless computing. Hydra utilizes VMs to handle steady workloads cost-effectively and leverages serverless elasticity to absorb traffic spikes. When compared to an all-VM deployment with Kubernetes auto-scaling, Hydra achieves a 62.4\% reduction in peak tail latency with a minimal 2.3\% increase in cost.",
author = "Dilina Dehigama and Shyam Jesalpura and Antonios Katsarakis and Marios Kogias and Rakesh Kumar and Boris Grot",
year = "2024",
month = apr,
day = "22",
language = "English",
pages = "1--8",
note = "The 2nd Workshop on SErverless Systems, Applications and MEthodologies, SESAME 2024 ; Conference date: 22-04-2024 Through 22-04-2024",
url = "https://sesame2024.github.io/",
}</pre>

<script>
  (function () {
    function fallbackCopy(text) {
      var el = document.createElement("textarea");
      el.value = text;
      el.setAttribute("readonly", "");
      el.style.position = "absolute";
      el.style.left = "-9999px";
      document.body.appendChild(el);
      el.select();
      document.execCommand("copy");
      document.body.removeChild(el);
    }

    function copyText(text) {
      if (navigator.clipboard && window.isSecureContext) {
        return navigator.clipboard.writeText(text);
      }
      fallbackCopy(text);
      return Promise.resolve();
    }

    document.addEventListener("click", function (event) {
      var btn = event.target.closest(".bibtex-copy");
      if (!btn) return;
      var targetId = btn.getAttribute("data-bibtex-target");
      var source = document.getElementById(targetId);
      if (!source) return;
      copyText(source.textContent.trim()).then(function () {
        var oldText = btn.textContent;
        btn.textContent = "Copied!";
        setTimeout(function () { btn.textContent = oldText; }, 1200);
      });
    });
  })();
</script>

<style>
  .section {
    padding-left: 1em;
  }

  .section-item {
    margin-bottom: 1.75em;
  }

  .p-no-margin-bottom {
    margin-bottom: 0 !important;
  }

  .btn-disabled {
    opacity: 0.6;
    pointer-events: none;
    cursor: not-allowed;
  }
</style>
