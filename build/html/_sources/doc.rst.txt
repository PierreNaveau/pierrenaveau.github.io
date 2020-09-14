.. sphinxTest documentation master file, created by
   sphinx-quickstart on Fri Sep  4 18:04:08 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.
   
.. toctree::
   :maxdepth: 2
   :caption: Contents:


1. Introduction
===============
itsme® is a trusted identity provider allowing partners to use verified identities for authentication and authorization on web desktop, mobile web or mobile applications.

The objective of this document is to provide all the information needed to integrate the **Authentication** service using the `OpenID Connect Core 1.0 specifications <http://openid.net/specs/openid-connect-core-1_0.html/>`_.

.. content-tabs::

    .. tab-container:: tab1
        :title: Authentication

        Here comes the example for authentication

    .. tab-container:: tab2
        :title: Confirm

        And here we have some specific text for a confirm

2. Prerequisite
===============

Before you start integrating itsme®, you MUST create an organisation on the following url: https://docs.google.com/forms/d/e/1FAIpQLSdyfhKiiehNg4DhFzhQeHaj9EG2VeFoyPNVaI-TSwnG5WlFfw/viewform.

Once there, you will need to fill out a basic form with the following questions:

    * Contact details such as your email, name, phone number.
    * Organisation details as shown on the company register for your jurisdiction.
    * Information about the project you want to set-up and the use case you have in mind.
    * itsme® terms and conditions. If you require a copy of this please contact onboarding@itsme.be.

Our onboarding team will review your project and get in touch within 3 days with a "client_id" and a "service_code" which need to be added in your configuration. Meanwhile, this should not prevent you from starting your integration.


3. Integration guide
====================

Our itsme® app can be seamlessly be integrated with your web desktop, mobile web or mobile application so you can perform secure identity checks.

Technical overview

itsme® integration is based on the Authorization Code Flow of OpenID Connect 1.0. The Authorization Code Flow goes through the steps as defined in OpenID Connect Core Authorization Code Flow Steps, depicted in the following diagram.

.. admonition:: Tip

        OpenID Connect provides certified libraries, products, and tools which could help you integrating the itsme® service. For more information, please visit the official webpage: https://openid.net/developers/libraries/. 


