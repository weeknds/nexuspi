# NexusPi - Web Frontend

This repository contains the web frontend for the NexusPi iOS app, a marketplace built on Pi Network.

## Purpose

This web presence serves several purposes:

1. Satisfy Pi Network hosting requirements for app development
2. Provide a landing page for the NexusPi iOS app
3. Host the privacy policy and terms of service required by Pi Network
4. Serve as a deep link destination for the app

## Structure

- `index.html`: Main landing page
- `policies/`: Directory containing legal documents
  - `privacy-policy.md`: Privacy policy required by Pi Network
  - `terms-of-service.md`: Terms of service

## Setup for GitHub Pages

1. Create a new GitHub repository named "nexuspi"
2. Push this code to the repository
3. Enable GitHub Pages in the repository settings
4. Configure it to serve from the main branch
5. Access your site at `https://your-username.github.io/nexuspi/`

## Pi Network Integration

This web frontend satisfies the Pi Network app requirements for:

1. **Configure App's Development URL**: Use `https://your-username.github.io/nexuspi/`
2. **Add Privacy Policy**: Available at `https://your-username.github.io/nexuspi/policies/privacy-policy.html`
3. **Validate Domain Ownership**: Follow Pi Network instructions to add a validation file
4. **Add a PiNet subdomain**: Optional for additional discoverability

## Customization

Before publishing, customize:

1. Replace `your-username` in all URLs with your actual GitHub username
2. Update contact email in the privacy policy and terms of service
3. Add your jurisdiction in the terms of service
4. Update any app store links when available
5. Customize styles and content as desired

## Integration with iOS App

The companion iOS app uses CloudKit for backend storage. This web frontend provides the necessary web presence for Pi Network requirements without needing to implement the backend functionality in web form. 