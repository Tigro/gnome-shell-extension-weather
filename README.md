## gnome-shell-extension-weather

gnome-shell-extension-weather is a simple extension for displaying weather notifications in Gnome Shell.

Currently, the weather report including forecast for today and tomorrow is fetched from [Yahoo](http://weather.yahoo.com/).

### Screenshots

![Screenshot](https://github.com/ecyrbe/gnome-shell-extension-weather/raw/master/data/screenshot.png)

And with french translation:  

![Screenshot](https://github.com/ecyrbe/gnome-shell-extension-weather/raw/master/data/screenshot2.png)

### Installation

From the command line

1. ./autogen.sh --prefix="/usr"
2. make
3. sudo make install
  
That's it!

### Configuration

Gnome extension weather use gsettings to save your configuration. you can use dconf-editor or gsettings from the command line to modify some parameters

#### Location (cf [WOEID](http://developer.yahoo.com/geo/geoplanet/guide/concepts.html))

You can specify your location buy using this command:

```bash
gsettings set org.gnome.shell.extensions.weather woeid 'your location'
```

#### Temperature units (optional, celsius by default)

You can modify the temperature unit with the following command

```bash
 gsettings set org.gnome.shell.extensions.weather unit 'celsius'
 ```
 or  

```bash
gsettings set org.gnome.shell.extensions.weather unit 'fahrenheit'
```

#### Displayed location (optional)

Sometimes your woeid location isn't quite right. it's the next major city around. to customise the displayed city you can type :

```bash
gsettings set org.gnome.shell.extensions.weather city 'your city'
```
### Restart Gnome-Shell

Don't forget to restart Gnome-Shell

1. Restart Gnome Shell (`[Alt]+[F2]`, `r`)
2. Fork this project as you like

### Licence

Copyright (C) 2011
Ecyrbe <ecyrbe+spam@gmail.com>,
Timur Kristóf <venemo@msn.com>,
Elad Alfassa <elad@fedoraproject.org>,
Simon Legner <Simon.Legner@gmail.com>

This file is part of gnome-shell-extension-weather.

gnome-shell-extension-weather is free software: you can redistribute it and/or modify it under the terms of the **GNU General Public License as published by the Free Software Foundation, either version 3** of the License, or (at your option) any later version.

gnome-shell-extension-weather is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with gnome-shell-extension-weather.  If not, see <http://www.gnu.org/licenses/>.

