## Blue Flute - How to Install:

* php composer.phar create-project laravel/laravel project_name
* cd project_name
* git init
* git add
* git commit -m "0"
* git remote add origin https://www.github.com/username/project_name.git
* git branch -M main
* git push origin main

#### About - Project Blue Flute:

* Blue Flute is a Demo / Sample Laravel to Vercel Deployment Workflow

#### Vercel JSON Package File:

* Sample Vercel JSON Package file below..

``
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
``

#### Sample Index PHP File Content below:

``
Require_Once($_SERVER["DOCUMENT_ROOT"].("/public/index.php"));
``

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
( C ) - [BinaryKore](https://github.com/binarykore), 09225205353