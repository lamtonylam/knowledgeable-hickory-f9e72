---
title: Home
layout: PageLayout
sections:
  - elementId: ''
    showDate: false
    showAuthor: false
    showExcerpt: false
    variant: variant-a
    actions:
      - type: Button
        label: View All
        altText: View All Posts
        url: /blog
        style: primary
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-12
          - pb-12
          - pl-4
          - pr-4
        justifyContent: center
      title:
        textAlign: center
      subtitle:
        textAlign: center
      actions:
        justifyContent: center
    title: Blogi
    colors: colors-a
    recentCount: 6
    type: RecentPostsSection
  - elementId: ''
    colors: colors-a
    quote: |
      “Fiksu mies käy kotona vessassa, fiksumpi mies käy töissä vessassa”
    name: '- Joku jäbä salee'
    title: '"Asiantuntija"'
    backgroundImage: null
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-36
          - pb-36
          - pl-4
          - pr-4
        justifyContent: center
      quote:
        textAlign: center
      name:
        fontWeight: 400
        fontStyle: normal
        textAlign: center
      title:
        fontWeight: 400
        fontStyle: normal
        textAlign: center
    type: QuoteSection
  - elementId: ''
    colors: colors-h
    backgroundSize: full
    title: HALOO ONKO ASIAA?
    text: |
      Jätä viesti sit.
    form:
      type: FormBlock
      variant: variant-a
      elementId: contact-form
      action: /.netlify/functions/submission_created
      destination: ''
      fields:
        - type: TextFormControl
          name: name
          label: Name
          placeholder: Your name
          isRequired: 'true'
          width: 1/2
        - type: EmailFormControl
          name: email
          label: Email
          placeholder: Your email
          isRequired: 'true'
          width: 1/2
        - name: Viesti
          label: Viesti
          hideLabel: false
          placeholder: Viesti
          isRequired: false
          width: full
          type: TextFormControl
      submitLabel: Send Message
    media:
      url: /images/48ACD.png
      altText: altText of the image
      caption: Caption of the image
      elementId: ''
      styles:
        self:
          opacity: 100
      type: ImageBlock
    styles:
      self:
        height: auto
        width: narrow
        margin:
          - mt-0
          - mb-0
          - ml-0
          - mr-0
        padding:
          - pt-12
          - pb-12
          - pl-4
          - pr-4
        alignItems: center
        justifyContent: center
        flexDirection: row
      title:
        textAlign: left
      text:
        textAlign: left
    type: ContactSection
---
