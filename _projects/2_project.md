---
layout: page
title: MoviesFeed
description: iOS app demonstrating TDD, clean architecture
img:
importance: 2
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

.appshot-wide {
  max-width: 800px; /* or any size that fits your page */
  width: 100%;
  border-radius: 12px; /* maybe smaller radius for big diagrams */
  box-shadow: 0 16px 40px rgba(0,0,0,.05);
}

.shot-caption{
  max-width:260px;             /* keep caption same width as image */
  margin-top:.5rem;
  text-align:center;
  color:#6c757d;
  font-size:.9rem;
}
</style>

> An iOS application built to demonstrate effective development techniques with a focus on **Test-Driven Development (TDD)**, **Clean Architecture**, **reusability**, and **maintainability**.

**GitHub repository:** [aekimov/AEFeed](https://github.com/aekimov/AEFeed)

---

## Overview

Showcases:

- Online & offline movie feed support
- Local caching with timestamp validation
- Review loading for movies
- Separation of concerns through Clean Architecture
- MVP UI pattern with clear loading states

API token from [The Movie Database](https://www.themoviedb.org/documentation/api) is needed to run the app.

---

## Key Features

**1. Always up-to-date online feed**  
When online, automatically fetch the latest movie feed to ensure a smooth, fresh experience.

**2. Offline-first experience**  
When offline, load the last saved feed from cache, so you can still browse even without internet.

**3. Movie reviews**  
Each movie can display a feed of reviews, offering valuable insight before you decide what to watch.

---

<div class="row g-spot section-spacer">
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/mf_1.png" title="Feed View" class="appshot" %}
  </div>
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/mf_2.png" title="Reviews View" class="appshot" %}
  </div>
</div>

## Dependency Diagram

<div class="row g-spot section-spacer">
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/diagram.png" title="Dependency diagram" class="appshot-wide" %}
  </div>
</div>

---

## MVP UI — Loading State Example

<div class="row g-spot section-spacer">
  <div class="col-sm mt-3">
    {% include figure.liquid path="assets/img/example-mvp.png" title="MVP loading state example" class="appshot-wide" %}
  </div>
</div>

---

## Technical Highlights

- **Architecture:** Clean Architecture with clear boundaries
- **Pattern:** Model-View-Presenter (MVP)
- **Testing:** Fully TDD-driven with isolated feature tests
- **Caching:** Local persistence with CoreData for feed and images, with expiry rules
- **Networking:** URLSession-based HTTP client with dependency injection

---
