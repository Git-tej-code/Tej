# Deploy a Package

**Who can do this**

* Platform Admin
* Power User (with deployment permission)

&#x20;

**Prerequisites**

* Package must be Locked
* Target environment must be available

&#x20;

**Supported Environment Transitions**

* Dev → QA
* QA → UAT
* UAT → QA
* QA → Dev

&#x20;

**Steps**

1. Open Version Control → Packages
2. Select the locked package
3. Click Deploy
4. Choose target environment
5. Confirm deployment

&#x20;

**What Happens Next**

* Entire package is deployed together
* All included processes become active
* Deployment event is logged

&#x20;

**Important Notes**

* Deployment is package-level only
* Individual processes cannot be deployed
* Rollback requires a different package/version

&#x20;

📸 Screenshot Required

* Deployment dialog
* Environment selector
