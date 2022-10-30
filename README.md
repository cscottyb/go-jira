# GoJira: Jira MacOS App with Dark Mode 
![alt text](https://github.com/cscottyb/gojira/blob/main/img/roadmap.png "screenshot of roadmap")


## Features
- Dark Mode that respects System theme
- Standalone App just for Jira. Jira doesn't need to clutter your browser
- Free Custom icon set that fits the look of MacOS icon design
- Small CSS files that can be used in your browser CSS injection extension. 

## Installation
### Simple
- Download the app from this project's Github Releases page.
- Move `GoJira.app` to your Applications folder. 

### Custom
#### Requirements
- Nativefier: An application
- (optional) png-to-icns: To convert 1024x1024 `.png` files into `.icns` files. 


#### Procedures
- Clone this project to your Mac
- open root folder of the project in Terminal
- Run command: REPLACE the ####### with your Atlassain.net subdomain. Your organization my have a different URL. Log into your account and use the URL that appears in your address bar. 
```
nativefier --name 'GoJira' 'https://#######.atlassian.net/jira/your-work' --inject style.css --title-bar-style 'hiddenInset' -i ./icon/gojira-icon-dark.icns
```
- The app is located in the output created in the root directory. 
- Drag and drop the `Gojira.app` into the Applications Folder. 
- Open the app from the Applications folder and pin the app into your Dock. 

#### Customization
- Change the `--name` value to whatever you want. 
- You can use any `.icns` file that is 1024x1024 in the icon folder or your own. 
	- GoJira Variants: Black, Dark, Light, and White

## Do you just want the the CSS instead for your browser's CSS injector plugin?
Use the `style-injector.css` file. 

I used the `Cascade` Extension for Safari and `Stylus` Extension/Plugin for Chromium Browsers and Firefox. 


## Disclaimer
I am not affiliated with Jira; please support the official method of using Jira. This software is provide to you as is and I'm not liable for damages stated in the MIT license. Licenses for Nativefier and Chromium are located in the `licenses` folder. This application is to is just a Electron wrapper for a browser window. 


### Bugs
- Sometimes the Nativefier crash after a long session. Save your work. 