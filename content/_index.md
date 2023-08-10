---
# Leave the homepage title empty to use the site title
title:
date: 2023-08-09
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Graduate Student
          company: MIT
          company_url: ''
          company_logo: MIT_logo
          location: Cambridge, MA, USA
          date_start: '2020-09-01'
          date_end: ''
          description: Materials Science and Engineering. Research topics - Magnetic nanotransducers, Surface Chemistry, Systemic Delivery, Neuromodulation
        - title: Research Engineer
          company: IHI Corporation
          company_url: ''
          company_logo: 
          location: Yokohama, JP
          date_start: '2015-04-01'
          date_end: '2020-07-31'
          description: Topics - Materials for batteries, fuel cells. Nd magnets. Permendur. Characterization (XRD, Battery properties, Magnetic properties)
        - title: Graduate Student (Master)
          company: University of Tokyo
          company_url: ''
          company_logo: UT_logo
          location: Tokyo, JP
          date_start: '2013-04-01'
          date_end: '2015-03-31'
          description: Materials Science and Engineering. Research topic - Growth process of quasicrystals
        - title: Undergraduate Student
          company: University of Tokyo
          company_url: ''
          company_logo: UT
          location: Tokyo, JP
          date_start: '2009-04-01'
          date_end: '2013-03-31'
          description: Materials Science and Engineering.
    design:
      columns: '2'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text:
      # Contact (add or remove contact options as necessary)
      email: keinagao@mit.edu
      autolink: true
      # Email form provider
    design:
      columns: '2'
---
