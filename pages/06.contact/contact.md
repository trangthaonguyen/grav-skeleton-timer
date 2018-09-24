---
title: Contact With Me
menu: Contact

map: 
  title: Find Us
  content: Si aute quis eu proident o cupidatat ne anim nescius, et est praesentibus, o quorum vidisse expetendis, nostrud eram quibusdam ad nam nostrud ubi.
  iframe: <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3651.277552998015!2d90.3678744!3d23.773128800000002!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3755c0ae4adf3cb9%3A0x7f2cf443b764e4a4!2sShishu+Mela!5e0!3m2!1sen!2s!4v1435516022247" width="100%" height="400" frameborder="0" style="border:0" allowfullscreen></iframe>
      
items: 
  - 
    classes: address wow fadeInLeft
    icon: ion-ios-location-outline
    content: 125 , Kings Street,Melbourne <br>United Kingdom,600562
  - 
    classes: address wow fadeInLeft
    icon: ion-ios-location-outline
    content: 125 , Kings Street,Melbourne <br>United Kingdom,600562
  - 
    classes: email wow fadeInLeft
    icon: ion-ios-email-outline
    content: support@themefisher.com<br>support@themefisher.com
  - 
    classes: phone wow fadeInLeft
    icon: ion-ios-telephone-outline
    content: +07 052 245 022<br>+07 999 999 999

form:
    name: contact

    fields:
        - name: name
          label: Name
          show_label: false
          placeholder: Your Name
          autocomplete: on
          classes: form-control
          type: text
          validate:
            required: true

        - name: email
          label: Email
          show_label: false
          placeholder: Your Email
          type: email
          classes: form-control
          validate:
            required: true

        - name: subject
          label: Subject
          show_label: false
          placeholder: Subject
          autocomplete: on
          classes: form-control
          type: text
          validate:
            required: true
            

        - name: message
          label: Message
          show_label: false
          classes: form-control
          placeholder: Message
          type: textarea
          rows: 6
          validate:
            required: true

    buttons:
        - type: submit
          value: Send Message
          classes: btn btn-default btn-send

    process:
        - email:
            subject: "[Site Contact Form] {{ form.value.name|e }}"
            body: "{% include 'forms/data.html.twig' %}"
            from: '{{ config.plugins.email.from }}'
            to: ['{{ config.plugins.email.to }}', '{{ form.value.email }}']
        - save:
            fileprefix: contact-
            dateformat: Ymd-His-u
            extension: txt
            body: "{% include 'forms/data.txt.twig' %}"
        - message: Thank you for getting in touch!
        - display: thankyou
---
Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolore, ea! consectetur adipisicing elit. Dolore, ea!