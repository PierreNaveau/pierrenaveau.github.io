.. sphinxTest documentation master file, created by
   sphinx-quickstart on Fri Sep  4 18:04:08 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.
   
.. toctree::
   :maxdepth: 2
   :caption: Contents:


1. Integration Sequence
=======================
itsme® is a trusted identity provider allowing partners to use verified identities for authentication and authorization on web desktop, mobile web or mobile applications.

The objective of this document is to provide all the information needed to integrate the **Authentication** service using the `OpenID Connect Core 1.0 specifications <http://openid.net/specs/openid-connect-core-1_0.html/>`_.

.. content-tabs::

    .. tab-container:: tab1
        :title: Authentication

        Here comes the example for authentication

    .. tab-container:: tab2
        :title: Confirm

        And here we have some specific text for a confirm

Integration Sequence
=======================

itsme® integration is based on the Authorization Code Flow of OpenID Connect 1.0. The Authorization Code Flow goes through the steps as defined in OpenID Connect Core Authorization Code Flow Steps, depicted in the following diagram:

.. image:: https://belgianmobileid.github.io/slate/OpenID_Login_SeqDiag.png
  :width: 400
  :alt: Sequence diagram

The integration steps, with linked code-level documentation are:


    1. Add itsme® button to your front-end page so the User can indicate he wishes to authenticate with itsme®: itsme® button specifications.
    2. Create the Authorization Request to authenticate the User. This request will redirect the User to the itsme® Front-End. itsme® then authenticates the User by asking him
        * to enter his phone number on the itsme® OpenID web page
        * authorize the release of some information to your application
        * to provide his credentials (itsme® code or fingerprint or FaceID)

    It is also in this Authorization Request that you will be able to request claims about the User and the Authentication event

    3. Collect the Authorization Code and redirect the user to your mobile or web application once the User has authorized the request and has been authenticated,
    4. Exchange the Authorization Code for an ID Token (e.g. identifying the User) and an Access Token.
    5. Request the additional User information from the itsme® userInfo Endpoint by presenting the Access Token obtained in the previous step.
    6. Confirm the success of the operation and display a success message.

If a user doesn't have the itsme® app, they'll be redirected to a mobile website with more information and download links.

3. Integration guide
====================

Our itsme® app can be seamlessly be integrated with your web desktop, mobile web or mobile application so you can perform secure identity checks.

Technical overview

itsme® integration is based on the Authorization Code Flow of OpenID Connect 1.0. The Authorization Code Flow goes through the steps as defined in OpenID Connect Core Authorization Code Flow Steps, depicted in the following diagram.

.. admonition:: Tip

        OpenID Connect provides certified libraries, products, and tools which could help you integrating the itsme® service. For more information, please visit the official webpage: https://openid.net/developers/libraries/. 


