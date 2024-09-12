# What is PWA- Progressive Web APP - 

PWA Apps are apps you can server from the web server without the need of app store

PWA apps are not from the play store rather a web browser app.


Project- PWA APP MANIFEST

- Serve and run on web app
- Work on the user interface
- Create installation meta data
- Make it offline available
- Prepare it for App Store distribution


## Using Service Worker

- The HTML registers a Service Worker
- The Service Worker installs some resources
- The browser download resources on demand, they can be served from the SW or the server


## UI Interface

Material Icon

## Steps in Making a PWA 

(Guideline to be seen on the Browser > Application )

1. Set the app.webmanifest.json
The web app manifest is a json file. One manifest -one PWA

## PROPERTIES OF THE WEB MANIFEST

 "name": "DevPad Experts, the ideal PWA to master your craft",
    "short_name": "DevPad",
    "start_url": "./?utm_source=pwa",
    "orientation": "landscape",
    "theme_color": "#ffc252", 
    "scope": "./",
    "display": "standalone",
    "icons":

1. name

2. start_url

3. orientation

4. Theme Color - never use gradient or hsla color type
- Set the theme-color on the html header as you can use media="" for light or dark mode.

5. Scope - Scope defines what is inside the internal - sub domain or external domain
. - "./" this could be a limitation in the PWA. Having different domains where the user have to install different apps could be a problem. Kepp everything under one domain.
- Just like opening Google Sign in on Tinder - this will take you to another domain - accounts.google.com - this is called an inner browser. You are still in the Tinder app. 
- There are inner browser in every PWA app that goes out from your main domain to another doamin but can still go out. External link can as well enable inner browser.

Main Question - Can the start url be in another domain - Answer is No- The start url must be in the same domain with the webmanifest.

The webmanifest tag defines the 

6. Display - (Display Modes on Android) this is one of the important property in PWA because without it you cannot have PWA
   - Standalone - You have to set your display - standalone - You have the theme color on the status bar
   - Minimal UI - (Sqooch) - renders a larger Nav bar - you see the current UI, alittle menu and hamburger where there 
- Fullscreen - 




7. icons - the only icon supported is png - no svg unless reset the sizes.
8. PWA ICONS ON ANDROID

#### Maskable Icons - Adaptive Icons since Android 8
What is a Maskable Icon - Is a centrally positioned circle with radius 40% of the icons's width.
100% width, 100%height with 40% radius
- circle - square
Icons App Manifest Recommended Sizes
-384 * 384, 1024*1024
192*192, 512*512


-Example
 "src": "./icons/icon-maskable.png",
            "sizes": "512x512",
            "type": "image/png",
            "purpose": "maskable"



- Simpler versions: 96*96
To open PWA on a web server
- npx serve .

## Types of PWA Apps

Squoosh
StarBucks

Tinder

## App Development Approaches

With PWA there is no native development or hybrid development. PWA works also available in browser and as a device specific app either in Android or desktop or IoS package.

With PWA there is no need installation of SDK

Most important aspects of PWA are
- Link and Discoverability
- Esy To Deploy
- Easy To Update
- Standard Tools
- Offline Access
- Standalone icons
- Operating system Integration
- High Performance and UX

## PWA Support Browsers


## PWA Components

Lighthouse 
- Available as a CLI and Dev Tools
- It tests your website agianst PWA criteria