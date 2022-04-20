<template>
  <!DOCTYPE html>
  <html>
    <head> </head>
    <body id="page-top">
      <!-- Navigation-->
      <NavigationBar />
      <!-- Masthead-->
      <MastHead />
      <!-- Services-->
      <ServicesSection />
      <!-- About-->
      <AboutSection />
      <!-- Clients-->
      <!-- <ClientsSection /> -->
      <!-- Contact-->
      <ContactSection />
      <!-- Footer-->
      <FooterSection />
    </body>
  </html>
</template>

<script lang="ts">
/* eslint-disable no-new */
import { ScrollSpy } from 'bootstrap'

export default {
  mounted() {
    /*!
     * Start Bootstrap - Agency v7.0.10 (https://startbootstrap.com/theme/agency)
     * Copyright 2013-2021 Start Bootstrap
     * Licensed under MIT (https://github.com/StartBootstrap/startbootstrap-agency/blob/master/LICENSE)
     */
    //
    // Scripts
    //

    // Navbar shrink function
    const navbarShrink = function () {
      const navbarCollapsible = document.body.querySelector('#mainNav')
      if (!navbarCollapsible) {
        return
      }
      if (window.scrollY === 0) {
        navbarCollapsible.classList.remove('navbar-shrink')
      } else {
        navbarCollapsible.classList.add('navbar-shrink')
      }
    }

    // Shrink the navbar
    navbarShrink()

    // Shrink the navbar when page is scrolled
    document.addEventListener('scroll', navbarShrink)

    // Activate Bootstrap scrollspy on the main nav element
    const mainNav = document.body.querySelector('#mainNav')
    if (mainNav) {
      new ScrollSpy(document.body, {
        target: '#mainNav',
        offset: 74,
      })
    }

    // Collapse responsive navbar when toggler is visible
    const navbarToggler: HTMLElement =
      document.body.querySelector('.navbar-toggler') ?? new HTMLElement()
    const responsiveNavItems = [].slice.call(
      document.querySelectorAll('#navbarResponsive .nav-link')
    )
    responsiveNavItems.forEach(function (responsiveNavItem: HTMLElement) {
      responsiveNavItem.addEventListener('click', () => {
        if (window.getComputedStyle(navbarToggler).display !== 'none') {
          navbarToggler.click()
        }
      })
    })
  },
}
</script>
