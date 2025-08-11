---
layout: page
title: CreditCalc
description: Convenient and accurate loan calculator
img:
importance: 3
category: mobile development
related_publications: false
---

<style>
  /* Smaller, card-like screenshots */
  .row.g-spot > .col-sm{
  display:flex;
  flex-direction: column;      /* stack image + caption */
  align-items: center;         /* center them */
}

.appshot { max-width:260px; width:100%; border-radius:28px; box-shadow:0 16px 40px rgba(0,0,0,.05); }

.shot-caption{
  max-width:260px;             /* keep caption same width as image */
  margin-top:.5rem;
  text-align:center;
  color:#6c757d;
  font-size:.9rem;
}

</style>

---

## Overview & tracking

Track multiple credits, plan advance (extra) repayments, choose how they apply (term or payment reduction), and instantly see the savings and new payoff date. A detailed amortization schedule keeps every payment transparent.

Create and manage several loans at once. See next payment, total paid, and remaining balance at a glance.

<div class="row g-spot section-spacer">
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/cc_1.png" class="appshot" %}
    <div class="shot-caption">Credits list — mortgage and car loan with progress</div>
  </div>
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/cc_2.png" class="appshot" %}
    <div class="shot-caption">Loan details — rate, totals, schedule & advance payment</div>
  </div>
</div>

---

## Plan extra repayments & see impact

Add an advance repayment, choose **Term reduction** or **Payment reduction**, and preview exactly how much interest you save and how the payoff date changes.

<div class="row g-spot section-spacer">
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/cc_3.png" class="appshot" %}
    <div class="shot-caption">Advance payment input — immediate savings preview</div>
  </div>
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/cc_4.png" class="appshot" %}
    <div class="shot-caption">Full amortization schedule — payment, interest, principal, balance</div>
  </div>
</div>
