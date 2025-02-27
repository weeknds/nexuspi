# Pi Network Integration Guide for NexusPi

This guide will walk you through the steps to complete the Pi Network integration for your NexusPi app.

## Prerequisites

Before you begin:

1. Create a Pi Network developer account at [developers.minepi.com](https://developers.minepi.com)
2. Set up your GitHub repository and GitHub Pages as described in GITHUB-SETUP.md
3. Ensure your app code is properly updated with your GitHub Pages URLs

## 1. Configure App's Development URL

1. Log in to the [Pi Network Developer Portal](https://developers.minepi.com)
2. Select your app from the dashboard
3. Navigate to the "App Details" section
4. Set the "Development URL" to your GitHub Pages URL: `https://YOUR_GITHUB_USERNAME.github.io/nexuspi/`
5. Save the changes

## 2. Add a Privacy Policy URL

1. In the App Details section of the Pi Developer Portal
2. Set the "Privacy Policy URL" to: `https://YOUR_GITHUB_USERNAME.github.io/nexuspi/policies/privacy-policy.html`
3. Save the changes

## 3. Validate Domain Ownership

Pi Network requires you to validate that you own the domain you're using:

1. Go to the "Domain Validation" section in the developer portal
2. Follow the instructions to download or copy the content of the validation file
3. Create or update the `.well-known/assetlinks.json` file in your GitHub repository with the provided content
4. Commit and push the changes to GitHub
5. Wait for GitHub Pages to deploy the changes (usually takes a few minutes)
6. Return to the Pi Developer Portal and click "Verify" to confirm domain ownership

## 4. Run Development App in the Sandbox

1. In the Pi Network Developer Portal, request access to the sandbox if not already granted
2. Install the Pi Network app on your iOS device
3. Go to the "Sandbox" tab in the Pi app
4. In the developer portal, select your app and click "Test in Sandbox"
5. Follow the instructions to test your app in the Pi Network sandbox environment
6. Verify that authentication works properly
7. Test the payment functionality in sandbox mode

## 5. Deploy App to Production Environment

Once your app is thoroughly tested in the sandbox environment:

1. Go to the "Production" section in the Pi Developer Portal
2. Request approval for production access
3. Provide any additional information requested during the review process
4. Wait for the Pi Network team to review and approve your app
5. Once approved, update the app code to use production APIs if needed

## 6. Add a PiNet subdomain (Optional)

For better discoverability, you can register a PiNet subdomain:

1. Go to the "PiNet Subdomain" section in the developer portal
2. Choose a subdomain name (e.g., `nexuspi.pi`)
3. Follow the instructions to configure the subdomain
4. Update your app with the new PiNet URL if applicable

## 7. Configure Payment Settings

For accepting payments through Pi Network:

1. Go to the "Payments" section in the developer portal
2. Configure the payment settings, including:
   - Payment recipient address
   - Transaction memo prefix (if required)
   - Callback URL for payment verification

## 8. Test Payment Flow

Make sure to thoroughly test the payment flow:

1. Test incomplete payment scenarios
2. Test canceled payment scenarios
3. Test successful payment scenarios
4. Verify that your app correctly handles all cases
5. Ensure proper record keeping of transactions

## 9. Submit for Production Review

Once all testing is complete:

1. Go to the "Submit for Review" section in the developer portal
2. Submit your app for production access
3. Provide detailed information about your app's functionality
4. Include testing instructions for the Pi Network review team
5. Wait for approval (this may take several days)

## 10. Monitoring & Maintenance

After your app is approved for production:

1. Regularly monitor the Pi Network developer dashboard
2. Keep your app updated with the latest Pi Network SDK changes
3. Respond promptly to any issues reported by users
4. Maintain compliance with Pi Network policies and guidelines

## Reference Information

- [Pi Network Developer Documentation](https://developers.minepi.com/doc/introduction)
- [Pi SDK Reference](https://developers.minepi.com/doc/sdkreference)
- [Pi Network Developer Forum](https://forum.minepi.com/c/developers/63)

Remember to regularly check for updates to the Pi Network platform and adjust your app accordingly. 