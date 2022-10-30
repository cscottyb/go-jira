# GoJira

![alt text](https://github.com/cscottyb/go-jira/blob/main/img/roadmap.png "screenshot of roadmap")

Jira MacOS App with Dark Mode 



## Features
- Dark Mode that respects System theme
- Jira doesn't need to live on your browser
- Custom icon set 
- Small CSS files

## Installation


### Simple
- Download the app from this project's Github Releases page.
- Move GoJira to your Applications folder

### Custom
#### Requirements
- Nativefier
- png-to-icns


#### Procedures
- Clone this project to your Mac
- open root folder of the project in Terminal
- Run command:
```
nativefier --name 'GoJira' 'https://#######.atlassian.net/jira/your-work' --inject style.css --title-bar-style 'hiddenInset' -i ./icon/gojira-icon-dark.icns
```

#### Customization
- Change the `--name` value
- You can use any `.icns` file that is 1024x1024
- 



## License

This software is provide to you as is and I'm not liable for damages stated in the MIT license. 