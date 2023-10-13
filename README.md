## About this Work Flow:

* Blue Flute is just a Demo Website / Project / Package which is the currently up to date version of Laravel to Vercel Deployment Workflow..

## Donations and Payments:
<details>
<summary>Donations and Payments</summary>
<p>
  <code>EWallet - Send Money</code>
  <br/>
  <br/>
  <code>Send Money: 09225205353 (GCash)</code>
  <br/>
  <code>Send Money: 09225205353 (Maya, soon)</code>
  <br/>
  <code>Send Money: 09225205353 (Coins PH)</code>
  <br/>
  <code>Send Money: 09225205353 (Palawan Pay)</code>
  <br/>
  <code>Remittance: 09225205353 (7/11 > GCash / Coins PH / Maya, soon)</code>
  <br/>
  <code>Remittance: 09225205353 (Palawan > GCash / Coins PH / Maya, soon)</code>
  <br/>
  <code>Remittance: 09225205353 (Cebuana > GCash / Coins PH / Maya, soon)</code>
  <br/>
  <code>Remittance: 09225205353 (MLhuillier > GCash / Coins PH / Maya, soon)</code>
</p>
<br/>
<p>
  <code>QR Code (GCash):</code>
</p>
<p>
  <img src="https://cdn.snowkel.us/image/redirect/gcash"></img>
</p>
</details>

## Blue Flute - How to Install:

* php composer.phar create-project laravel/laravel project_name
* cd project_name
* git init
* git add
* git commit -m "0"
* git remote add origin https://www.github.com/username/project_name.git
* git branch -M main
* git push origin main

#### Vercel JSON Package File:

* Sample Vercel JSON Package file below..

```php
{
	"version": 2,
	"framework": null,
    "functions": {
		"api/index.php": {
			"runtime": "snowkelus-php@0.2.0"
		}
	},
    "routes": [
        {
            "src": "/(.*)",
            "dest": "/api/index.php"
        }
    ],
    "env": {
        "APP_NAME": "Blue Flute Systems for PHP Laravel..",
        "APP_ENV": "production",
        "APP_DEBUG": "false",
        "APP_URL": "https://blueflute.vercel.app",
        "APP_CONFIG_CACHE": "/tmp/config.php",
        "APP_EVENTS_CACHE": "/tmp/events.php",
        "APP_PACKAGES_CACHE": "/tmp/packages.php",
        "APP_ROUTES_CACHE": "/tmp/routes.php",
        "APP_SERVICES_CACHE": "/tmp/services.php",
        "VIEW_COMPILED_PATH": "/tmp",
        "CACHE_DRIVER": "array",
        "LOG_CHANNEL": "stderr",
        "SESSION_DRIVER": "cookie",
        "VIEW_COMPILED_PATH": "/tmp/views",
        "SSR_TEMP_PATH": "/tmp/ssr",
        "NODE_PATH": "node"
    }
}
```

#### Sample Index PHP File Content below:

```php
Require_Once($_SERVER["DOCUMENT_ROOT"].("/public/index.php"));
```

#### Sample Vercel Ignore File Content below:

* Input this in the .vercelignore file:

``
/vendor
``

* Then the vendor folder which where the Packages are installed will be ignored from getting parsed

#### Output Directory, Vercel:

* First create an Empty Folder named "dist"
* Then input the Details before Deploying naming: "public" in Output Directory
* Then Deploy to Vercel (if it succeeds, then you're good to go)

#### Environment Variables:

* Generate an Environment Variable from "php artisan key:generate"
* Then Input these in the Environment Variables from Settings: APP_KEY:base64_APP_KEY


### Copyright since ( 2023 )
( C ) - [Binary Kore](https://github.com/binarykore), 09225205353