---
title: MVP Feature List
author: ojas
pubDatetime: 2025-05-01T04:06:31Z
slug: mvp-feature-list
featured: false
draft: false
tags:
  - planning
description:
  Our MVP feature list contains all the features we want in our MVP. We want to hit these goals but we also wanted to be a little ambitious here.
---

These are the features we decided to implement in the meeting on Friday, 30 April '25':

* Generating recourses using all the input provided - summarisation, flashcards, FAQs, Examples, DuoLingo Style Quizzes
    * FAQs are a differentiator feature where the user gets to save the questions they ask as a separate page where they can refer back to the question while revising
    * Examples (especially useful for mathematics) is when the AI will try to put the input into different contexts in real life or otherwise to provide a wider range of perspective to the user
    * DuoLingo style quizzes will remember what mistakes user makes and try to incorporate that in future quizzes.

* Multimodal Input - Text, Audio, PDF, Handwriting, Thought Dump
    * Thought dump feature will implement a new mode of input where user can record themselves/type unstructured informal notes right after or during the class. This will be considered as an entire mode in the model, however it should be treated as something in an informal format.

* Three creatively named modes
    * (Placeholder name) Easy Mode:
        * Based on the input, the resources will be instantly provided to the user (base level NoteBookLM Implementation)
    * (Placeholder name) Medium Mode:
        * Based on the input, a series of fill-in-the-blank style questions come up which need to be answered to unlock the entire list of resources.
        * The fill-in-the-blanks feature is a differentiator, it puts Nuclear apart from basic Quiz style testing.
        * Once the user "unlocks" the resources, they have access to all the resources to use.
    * (Placeholder name) Hard Mode:
        * Input initially not provided.
        * (base level Notion Implementation) Would be a clean feature-rich notetaking experience.
        * Features in this mode will include - LaTex formatting, markdown formatting, tables, pictures (through markdown), any quality of life features.
        * This will possibly be a free mode, so it's important to have a fluhed out UI and easy to use design.
        * Once the use finishes notetaking step, they are led to input screen where they can choose to add more inputs like lecture notes, or use their notes to generate the resources as mentioned above.


* Spotify Controls :)
