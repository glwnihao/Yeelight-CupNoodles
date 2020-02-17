# OverView

This document introduce how to integrate Yeelight products to third-party service or platform.

Yeelight supports OAuth2.0 with an authorization code flow by Mi Passport, providing all the information that third-party need to implement OAuth, such as Client ID, Client Secret, Authorization Endpoint and Token Exchange Endpoint.

Yeelight will provide a key for each third-party, and third-party need to put this key in the header of each request.

If the property change notify is required, third-party need to provide Property Change Report Endpoint.