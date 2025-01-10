---
# Leave the homepage title empty to use the site title
title: ''
date: 2025-01-01
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: About Me
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Assistant Professor
          company: School of Neurosscience, Virginia Tech
          company_url:
          company_logo: org-vt
          location: Blacksburg, Virginia
          date_start: '2021-07-10'
          date_end: ''
          description:
        - title: Postdoctoral Fellow
          company: Baraban Lab, Johns Hopkins University
          company_url: ''
          company_logo: org-jhusom
          location: Baltimore, Maryland
          date_start: '2015-06-01'
          date_end: '2021-07-09'
          description:
        - title: Postdoctoral Fellow
          company: Mathur Lab, University of Maryland
          company_url: ''
          company_logo: org-umb
          location: Baltimore, Maryland
          date_start: '2014-06-01'
          date_end: '2015-05-31'
          description:
        - title: PhD Candidate
          company: Frazer Lab, UT Health San Antonio
          company_url: ''
          company_logo: org-uthsa
          location: San Antonio, Texas
          date_start: '2008-09-01'
          date_end: '2014-05-31'
          description:
        - title: Junior Research Fellow
          company: Panicker Lab, National Centre for Biological Sciences
          company_url: ''
          company_logo:
          location: Bengaluru, India
          date_start: '2007-07-01'
          date_end: '2008-05-31'
          description:
    design:
      columns: '2'
  - block: collection
    id: news
    content:
      title: News
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
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project  
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: masonry
      # For Showcase view, flip alternate rows?
      flip_alt_rows: true
  - block: collection
    id: publications
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
      view: compact
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text:
      # Contact (add or remove contact options as necessary)
      email: aparnashah@vt.edu
      address:
        street: 210 Drillfield Drive
        city: Blacksburg
        region: VA
        postcode: '24060'
        country: United States
        country_code: US
      # Choose a map provider in `params.yaml` to show a map from these coordinates
#      coordinates:
#        latitude: '37.2259'
#        longitude: '-80.4234'  
      contact_links:
        - icon: bluesky
          icon_pack: fab
          name: Follow Me
          link: 'https://bsky.app/profile/neuromusings.bsky.social'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
          # Enable CAPTCHA challenge to reduce spam?
      #     captcha: false
    design:
      columns: '2'
---
