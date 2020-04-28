# Real Time

A boilerplate for real-time HTML/CSS/JS compilation from HAML/Sass/Coffee using Guard. 

To get started:

* git clone --depth 1 git@github.com:mahemoff/realtime.git your-project && cd your-project && rm -fr .git
* Install Ruby and run `bundle`
* Run `bin/realtime` and hit enter on the "guard >" prompt
* Run `bin/http` in another window

In your browser, open http://localhost:4848 to view the initial content. It should now be driven by your app/ folder, any changes you save will automatically re-compile the project. Optionally, you can follow the link from there to make your browser live-reload as you save source files.
