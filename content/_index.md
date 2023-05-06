---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: features
    id: skills
    content:
      title: Skills
      items:
        - name: AWS
          description: ⭐⭐⭐⭐
          icon: aws
          icon_pack: custom
        - name: Terraform
          description: ⭐⭐⭐⭐
          icon: terraform
          icon_pack: custom
        - name: Docker
          description: ⭐⭐⭐⭐
          icon: docker
          icon_pack: custom
        - name: Kubernetes
          description: ⭐⭐⭐⭐
          icon: k8s
          icon_pack: custom
        - name: Linux
          description: ⭐⭐⭐⭐
          icon: linux
          icon_pack: custom
        - name: Github ACtions 
          description: ⭐⭐⭐⭐
          icon: github-actions
          icon_pack: custom
        - name: Gitlab CI/CD
          description: ⭐⭐
          icon: gitlab
          icon_pack: custom
        - name: Azure
          description: ⭐
          icon: azure
          icon_pack: custom
        - name: Digital Ocean
          description: ⭐
          icon: digital
          icon_pack: custom
      
  - block: portfolio
    id: achievements
    content:
      title: Achievements
      filters:
        folders:
          - achievements
      default_button_index: 0
      buttons:
        - name: All
          tag: '*'
        - name: Certification
          tag:  certification
        - name: Award
          tag:  award

    design:
      columns: '1'
      view: showcase
      flip_alt_rows: false

  - block: experience
    id: experience
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
        - title: Associate DevOps Engineer
          company: Brain Station 23
          company_url: 'https://brainstation-23.com'
          company_logo: org
          location: Dhaka
          date_start: '2022-07-01'
          date_end: ''
          description: |2-
              Responsibilities include:

              * Collaboration
              * Continuous Integration and Deployment
              * Infrastructure Automation
              * Monitoring and Alerting
              * Performance Optimization
              * Security
              * Troubleshooting
        - title: DevOps Engineer Trainee
          company: Brain Station 23
          company_url: 'https://brainstation-23.com'
          company_logo: org
          location: Dhaka
          date_start: '2022-01-01'
          date_end: '2022-06-30'
          description: I completed an internship at Brain Station 23 where I gained hands-on experience with various DevOps technologies, such as Docker, AWS, Kubernetes, Grafana, Jenkins, Terraform, and Github Actions. This internship provided me with a solid foundation in cloud computing, containerization, and infrastructure management. I appreciated the company's commitment to helping young talent grow and develop their skills, and overall, the experience was a positive and valuable learning opportunity that has prepared me for a career in the tech industry.
    design:
      columns: '2'
  # - block: accomplishments
  #   content:
  #     # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
  #     title: 'Accomplish&shy;ments'
  #     subtitle:
  #     # Date format: https://wowchemy.com/docs/customization/#date-format
  #     date_format: Jan 2006
  #     # Accomplishments.
  #     #   Add/remove as many `item` blocks below as you like.
  #     #   `title`, `organization`, and `date_start` are the required parameters.
  #     #   Leave other parameters empty if not required.
  #     #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
  #     items:
  #       - certificate_url: https://www.coursera.org
  #         date_end: ''
  #         date_start: '2021-01-25'
  #         description: ''
  #         organization: Coursera
  #         organization_url: https://www.coursera.org
  #         title: Neural Networks and Deep Learning
  #         url: ''
  #       - certificate_url: https://www.edx.org
  #         date_end: ''
  #         date_start: '2021-01-01'
  #         description: Formulated informed blockchain models, hypotheses, and use cases.
  #         organization: edX
  #         organization_url: https://www.edx.org
  #         title: Blockchain Fundamentals
  #         url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
  #       - certificate_url: https://www.datacamp.com
  #         date_end: '2020-12-21'
  #         date_start: '2020-07-01'
  #         description: ''
  #         organization: DataCamp
  #         organization_url: https://www.datacamp.com
  #         title: 'Object-Oriented Programming in R'
  #         url: ''
  #   design:
  #     columns: '2'
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
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Industry Projects
          tag:  Industry Project
        - name: Personal Projects
          tag:  Personal Project
        - name: Academic Project
          tag:  Academic Project

    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  # - block: markdown
  #   content:
  #     title: Gallery
  #     subtitle: ''
  #     text: |-
  #       {{< gallery album="demo" >}}
  #   design:
  #     columns: '1'
  # - block: collection
  #   id: featured
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #   design:
  #     columns: '2'
  #     view: card
  # - block: collection
  #   content:
  #     title: Recent Publications
  #     text: |-
  #       {{% callout note %}}
  #       Quickly discover relevant content by [filtering publications](./publication/).
  #       {{% /callout %}}
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: true
  #   design:
  #     columns: '2'
  #     view: citation
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     columns: '2'
  #     view: compact
  # - block: tag_cloud
  #   content:
  #     title: Popular Topics
  #   design:
  #     columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Thank you for visiting my website! I'm always open to new opportunities and would love to hear from you. Whether you have a question, a project you'd like to collaborate on, or just want to say hello, feel free to reach out using the contact form below. I'll do my best to respond as soon as possible. Thank you for your interest!
      # Contact (add or remove contact options as necessary)
      email: purbo7512@gmail.com
      # phone: 888 888 88 88
      # appointment_url: 'https://calendly.com'
      # address:
      #   street: 450 Serra Mall
      #   city: Stanford
      #   region: CA
      #   postcode: '94305'
      #   country: United States
      #   country_code: US
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
      #   - 'Monday 10:00 to 13:00'
      #   - 'Wednesday 09:00 to 10:00'
      contact_links:
        - icon: facebook
          icon_pack: fab
          name: DM Me
          link: 'https://www.facebook.com/profile.php?id=100023648450150'
        # - icon: skype
        #   icon_pack: fab
        #   name: Skype Me
        #   link: 'skype:echo123?call'
        # - icon: video
        #   icon_pack: fas
        #   name: Zoom Me
        #   link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      # autolink: true
      # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
      #     # Enable CAPTCHA challenge to reduce spam?
      #     captcha: false
    design:
      columns: '2'
---
