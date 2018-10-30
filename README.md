# **mePAge**

This is a single page, single screen responsive site template
![screenshot](https://raw.githubusercontent.com/sethmacleod/aerial/master/images/screenshot.png)

# If you wanna run locally to make your changes and port it:
 
## Installation

- Required : Hugo0.5 [HUGO](https://gohugo.io)

Run the following commands inside the folder of your Hugo site:

	$ cd themes [ this is important !]
	$ git clone https://github.com/franbonafina/mePage.git

## Getting Started

After installation, you only need to configure the config.toml file and, if desired, change the background picture.

### The config file

Copy the config.toml file from the meSite folder into your root folder of your Hugo site. Change the fields as needed.

### To Run it:

    $ hugo --config theme.toml,config.toml
    $ hugo server

#### Change the background

`Should you choose to change the background, create a `/static/css/images` folder and add a picture named `bg.jpg`. For the best results, follow these instructions:

        Look for this line in css/style.css : 
            background: #348cb2 url("images/bg.jpg") bottom left;
        and use it to set the page background color, URL, and placement of
        your image. It should be as close to 1500px wide as you can get it.`


### Add custom js snippets

Should you choose to add custom js snippet, create a `layouts/partials` folder with `js.html` file and put your js code in this file.

This can be useful for adding [Google Analytics](https://gohugo.io/extras/analytics/). Just add `{{ template "_internal/google_analytics.html" . }}` to the file and configure the config file with your `googleAnalytics` tracking id.


