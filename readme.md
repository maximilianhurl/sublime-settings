# Sublime setup

This Repo contains some useful help on getting a fresh install of Sublime Text setup.

## Step 1 - Install package manager

First you need to install the sublime package controller which you can get from [https://sublime.wbond.net/](https://sublime.wbond.net/).

When this is done it should be relatively simple to install the following packages by pressing `ALT` + `SHIFT` + `P` and typing `install package`. 

#### Installed Packages:

    "Dayle Rees Color Schemes",
    "LESS",
    "Package Control",
    "SideBarEnhancements",
    "SublimeLinter",
    "Theme - Soda"
    

## Step 2 - Sublime settings

After you have installed all the packages you can add in your settings

#### Settings User:

	{
		"color_scheme": "Packages/Dayle Rees Color Schemes/Peacock.tmTheme",
		"font_face": "Menlo",
		"font_options":
		[
			"no_round"
		],
		"font_size": 12.0,
		"highlight_line": true,
		"ignored_packages":
		[
			"Vintage"
		],
		"open_files_in_new_window": false,
		"tab_size": 4,
		"theme": "Soda Dark.sublime-theme",
		"translate_tabs_to_spaces": true,
		"trim_trailing_white_space_on_save": true
	}

To install the colour scheme you need to select `Preferences -> Browse Packages` then download the colour scheme set from [https://github.com/daylerees/colour-schemes](https://github.com/daylerees/colour-schemes) into that directory.

#### Settings Python:

	{
	    "rulers": [80],
	    "tab_size": 4,
	    "trim_automatic_white_space": true,
	    "trim_trailing_white_space_on_save": true,
	
	    "pep8_ignore":
	    [
	        "E501",
	        "E128"
	    ]
	}

#### Sublime linter settings user

	{
	    "sublimelinter": true,
	    "sublimelinter_popup_errors_on_save": false,
	    "sublimelinter_delay": 0,
	    "sublimelinter_mark_style": "outline",
	    "javascript_linter": "jslint",
	    "jslint_options":
	    {
	        "browser": true,
	        "devel": true
	    },
	    "pep8_ignore":
	    [
	        "E501",
	        "E128"
	    ]
	}
	
	
## Step 3 - Install snippets

See the snippets directory for more information