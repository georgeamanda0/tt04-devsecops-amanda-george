# DIT637-TT04
# How to Run If Setup has been done

## Backend - ExpressJS
In a new terminal type: 
- `cd backend-expressjs`
- `npm install` 
- `npm run start`

## Frontend - React Native
In a new terminal type: 
- `cd frontend-reactnative`
- `npm install`
- `npx expo login`
- `npx expo start --tunnel`
5. Scan the QR Code with your mobile phone

# Setup
## Database - MongoDB Atlas
1. Create an account
2. Create DB copy MongoDB connection string

## Backend - ExpressJS
1. Go inside backend-expressjs folder create `.env` 
2. Follow the `example.env` file and paste the MongoDB connection string
3. In a new terminal type: 
- `cd backend-expressjs`
- `npm install` 
- `npm run start`
- make sure its allowed public access.
4. Copy the forwarded address

## Frontend - React Native
1. Create an Expo Go account and download in your Mobile Phone
2. Go inside frontend-reactnative folder create `.env` 
3. Follow the `example.env` file and paste the forwarded address of backend server
4. In a new terminal type: 
- `cd frontend-reactnative`
- `npm install`
- `npx expo login`
- `npx expo start --tunnel`
5. Scan the QR Code with your mobile phone

After completing these steps, you should be able to test your mobile app


## AI-Assisted Documentation: Automated Security Scanning 
Automated Security Scanning with GitHub Actions and OWASP ZAP: This project integrates OWASP ZAP into the CI/CD pipeline as a dedicated zap_scan job that runs automatically on every push to the main branch, using the zaproxy/action-baseline@v0.12.0 action with a containerized ZAP instance (ghcr.io/zaproxy/zaproxy:stable). The job performs a baseline scan against zapproxy.org, the ZAP website, and applies a custom rules file (.zap/rules.tsv) to tune which alerts are reported, filing the results as a ZAP Scan Baseline Report in the repository's Issues tab. When  shifting security testing earlier into the automated build process, we continuously uncover vulnerabilities during development instead of finding them after deployment. This proactive approach is key to creating a Smart and Secure System.