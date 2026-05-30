# vamsi-lwc-project

This repository is initialized as a Salesforce DX project for building Lightning Web Components (LWC) and deploying them to a Trailhead org.

## Getting started

1. Authorize your Trailhead org:

   ```bash
   sfdx auth:web:login -a trailorg
   ```

2. Deploy the sample component to your Trailhead org:

   ```bash
   sfdx force:source:deploy -p force-app -u trailorg
   ```

3. Open the org in your browser:

   ```bash
   sfdx org:open -u trailorg
   ```

## Project structure

- `sfdx-project.json` — Salesforce DX project config
- `force-app/main/default/lwc/helloWorld` — sample LWC component
- `.forceignore` — files ignored by Salesforce CLI

## Create a new Lightning Web Component

```bash
sfdx force:lightning:component:create -n myComponent -d force-app/main/default/lwc -t lwc
```

## Deploy changes

```bash
sfdx force:source:deploy -p force-app -u trailorg
```
