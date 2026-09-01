# Qibla Direction Privacy Policy

Static GitHub Pages privacy policy for:

- App: Qibla Direction
- Package: com.afaquekhan.qibladirection
- Repository name: qibladirection-privacy-policy

This follows the same GitHub Pages pattern previously used for NumberDrop.

## Fast path

Open PowerShell in this folder and run:

```powershell
Set-ExecutionPolicy -Scope Process Bypass
.\PREPARE_QIBLA_PRIVACY_POLICY.ps1
```

The script asks for:

1. GitHub username
2. Public support email

It fills the support email into both HTML pages and prepares the Git repository.

Create a PUBLIC GitHub repository named:

qibladirection-privacy-policy

Then push:

```powershell
git push -u origin main
```

In GitHub:

Settings -> Pages
Source: Deploy from a branch
Branch: main
Folder: /(root)
Save

Expected URL:

https://<github-username>.github.io/qibladirection-privacy-policy/privacy-policy.html

Use that URL in Google Play Console -> Privacy policy.

IMPORTANT
Google Play also requires a privacy policy link or text to be available within the app.
Before production release, verify Qibla Direction's Settings/Support screen exposes the policy.
If sealed 1.0.0 does not, add the privacy-policy link in a later versionCode rather than modifying the sealed 1.0.0 artifact.
