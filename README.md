# southern-edge-land-management-webpage

## Facebook Reviews

To display live Facebook reviews, update the `facebookReviewsConfig` object near the bottom of `index.html` with your Facebook page URLs and a secure `reviewsEndpoint`. The endpoint should proxy the Facebook Graph API server-side so access tokens are never exposed in the browser. Without that endpoint, the site will fall back to the featured testimonials.
