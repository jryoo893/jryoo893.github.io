---
layout: page
permalink: /project/
title: Project
nav: true
nav_order: 0
---

<style>
  .themes {
    margin: 0.5rem 0 3rem;
  }
  .theme {
    display: grid;
    grid-template-columns: minmax(0, 5fr) minmax(0, 7fr);
    gap: 2rem;
    align-items: center;
    padding: 2rem 0;
    border-top: 1px solid var(--global-divider-color);
  }
  .theme:last-child {
    border-bottom: 1px solid var(--global-divider-color);
  }
  .theme:nth-child(even) {
    grid-template-columns: minmax(0, 7fr) minmax(0, 5fr);
  }
  .theme:nth-child(even) .theme-media {
    order: 2;
  }
  .theme-media {
    margin: 0;
  }
  .theme-media img {
    display: block;
    width: 100%;
    aspect-ratio: 4 / 3;
    object-fit: cover;
    border-radius: 6px;
    background: #000;
  }
  .theme-number {
    font-size: 0.75rem;
    font-weight: 600;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--global-theme-color);
    margin-bottom: 0.3rem;
  }
  .theme-body h2 {
    font-size: 1.35rem;
    margin: 0 0 0.6rem;
  }
  .overview {
    margin: 1.5rem 0 0;
  }
  .overview p {
    margin-bottom: 0.9rem;
  }
  @media (max-width: 720px) {
    .theme:nth-child(even) {
      grid-template-columns: 1fr;
    }
    .theme {
      grid-template-columns: 1fr;
      gap: 1rem;
    }
    .theme:nth-child(even) .theme-media {
      order: 0;
    }
    .theme-media img {
      aspect-ratio: 16 / 9;
    }
  }
</style>

<div class="overview">

<p>My research covers computer architecture, memory systems, and operating systems, with
a focus on workload characterization. Current work spans energy-efficient and secure
memory systems, artificial intelligence with a focus on diffusion models, and AI in
computer science education.</p>

</div>

<div class="themes">

  <section class="theme">
    <figure class="theme-media">
      <img src="{{ '/assets/img/themes/memory-systems.jpg' | relative_url }}"
           alt="A single stacked DRAM die from a high-bandwidth memory (HBM) stack, photographed under magnification." loading="lazy" />
    </figure>
    <div class="theme-body">
      <div class="theme-number">Theme 01</div>
      <h2>Memory systems and computer architecture</h2>
      <p>DRAM subsystem research spans memory scheduling and refresh, protection against
      memory-level security vulnerabilities, and processing-in-memory architectures that
      compute inside DRAM. Address translation research focuses on TLB design for
      virtualized and GPU systems.</p>
    </div>
  </section>

  <section class="theme">
    <figure class="theme-media">
      <img src="{{ '/assets/img/themes/ai-systems.jpg' | relative_url }}"
           alt="A GPU package: a large GPU die surrounded by four stacked high-bandwidth memory chips on a silicon interposer." loading="lazy" />
    </figure>
    <div class="theme-body">
      <div class="theme-number">Theme 02</div>
      <h2>Artificial intelligence and diffusion models</h2>
      <p>Diffusion models are studied from the hardware up, including performance
      characterization of image, video, and 3D diffusion models across GPU architectures,
      activation sparsity in diffusion model layers, and training dynamics of
      temporal-attention heads in video diffusion transformers. Conditional diffusion models
      synthesize MRI from anatomical structure, lesions, and disease for neuroimaging
      applications. Large language model research targets memory-efficient serving.</p>
    </div>
  </section>


  <section class="theme">
    <figure class="theme-media">
      <img src="{{ '/assets/img/themes/cs-education.jpg' | relative_url }}"
           alt="A university student at a laptop in a classroom, talking through their work." loading="lazy" />
    </figure>
    <div class="theme-body">
      <div class="theme-number">Theme 03</div>
      <h2>AI in computer science education</h2>
      <p>AI tools for computer science education include multi-agent tutoring systems,
      AI-assisted quizzing, and knowledge-graph-based learning environments, designed and
      evaluated in real courses. Studies examine self-regulated learning, student
      disclosure of AI use, and assessment design when generative AI is widely
      available.</p>
    </div>
  </section>

</div>
