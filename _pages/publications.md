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
    <p class="p-no-margin-bottom"><strong>Spandana: Reconciling Strict SLOs with Low Cost under Fine-Grained Load Fluctuations</strong><br>
    D. Dehigama, S. Jesalpura, Z. Xu, M. Nemeth, M. Kogias, and B. Grot<br>
    <em>Accepted at SoCC, 2026</em> <span class="badge-new">New</span></p>
    <div class="button-group">
      <a href="#" class="btn btn--primary btn-disabled" aria-disabled="true">PDF (Add URL)</a>
      <button type="button" class="btn btn--primary bibtex-copy" data-bibtex-target="bibtex-spandana">Copy BibTeX</button>
    </div>
  </div>

  <div class="section-item">
    <p class="p-no-margin-bottom"><strong>Harmonizing Diverse Compute Resources for Efficiency</strong><br>
    D. Dehigama, S. Jesalpura, M. Kogias, and B. Grot<br>
    <em>HotInfra at SOSP, 2024</em></p>
    <div class="button-group">
      <a href="#" class="btn btn--primary btn-disabled" aria-disabled="true">PDF (Add URL)</a>
      <button type="button" class="btn btn--primary bibtex-copy" data-bibtex-target="bibtex-hotinfra">Copy BibTeX</button>
    </div>
  </div>

  <div class="section-item">
    <p class="p-no-margin-bottom"><strong>Composing Microservices and Serverless for Load Resilience</strong><br>
    D. Dehigama, S. Jesalpura, A. Katsarakis, M. Kogias, R. Kumar, and B. Grot<br>
    <em>SESAME at EuroSys, 2024</em></p>
    <div class="button-group">
      <a href="#" class="btn btn--primary btn-disabled" aria-disabled="true">PDF (Add URL)</a>
      <button type="button" class="btn btn--primary bibtex-copy" data-bibtex-target="bibtex-sesame">Copy BibTeX</button>
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

<pre id="bibtex-hotinfra" class="bibtex-source" hidden>@inproceedings{dehigama2024harmonizing,
  title     = {Harmonizing Diverse Compute Resources for Efficiency},
  author    = {Dehigama, Dilina and Jesalpura, Smit and Kogias, Marios and Grot, Boris},
  booktitle = {2nd Workshop on Hot Topics in System Infrastructure (HotInfra) at SOSP},
  year      = {2024}
}</pre>

<pre id="bibtex-sesame" class="bibtex-source" hidden>@inproceedings{dehigama2024composing,
  title     = {Composing Microservices and Serverless for Load Resilience},
  author    = {Dehigama, Dilina and Jesalpura, Smit and Katsarakis, Alexandros and Kogias, Marios and Kumar, Ravi and Grot, Boris},
  booktitle = {2nd Workshop on SErverless Systems, Applications and MEthodologies (SESAME) at EuroSys},
  year      = {2024}
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
