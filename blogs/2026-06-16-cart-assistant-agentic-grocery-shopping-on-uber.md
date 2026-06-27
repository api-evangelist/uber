---
title: "Cart Assistant: Agentic Grocery Shopping on Uber Eats"
url: "https://www.uber.com/us/en/blog/uber-cart-assistant/"
date: "2026-06-16"
author: "Anurag Biyani, Deepak Kumar Sahoo, Renato Beserra Sousa"
feed_url: "https://www.uber.com/blog/engineering/"
---
Uber's Cart Assistant lets Uber Eats users enter a prompt or upload an image and have the system generate a draft grocery cart to review and edit before ordering. It runs on a multi-prompt state graph architecture with eight stages: cart plan generation, candidate retrieval, semantic relevance judging, constraint enforcement, quantity selection, guardrails, cart assembly, and content refinement, combining focused LLM calls with deterministic APIs and validation layers. Development used evaluation-driven improvement with deterministic verification and LLM-as-a-judge assessments against synthetic and production-derived test cases.
