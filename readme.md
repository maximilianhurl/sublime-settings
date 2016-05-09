# Sublime setup

This Repo contains some useful help on getting a fresh install of Sublime Text setup.

## Step 1 - Install package manager

First you need to install the sublime package controller which you can get from [https://sublime.wbond.net/](https://sublime.wbond.net/).

When this is done it should be relatively simple to install the following packages by pressing `CMD` + `SHIFT` + `P` and typing `install package`.

#### Installed Packages:

    "Dayle Rees Color Schemes",
    "LESS",
    "SideBarEnhancements",
    "SublimeLinter",
    "MarkdownEditing",
    "Theme - Soda",
    "Theme - Spacegray",
    "Babel",
    "GitGutter",
    "Djaneiro"


## Step 2 - Sublime settings

After you have installed all the packages you can add in your preferences -> settings - user

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
		"theme": "Spacegray.sublime-theme",
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

#### Settings JS

	{
    	"rulers": [120],
    	"tab_size": 4,
		"extensions":
		[
			"js"
		]
	}



#### Sublime linter settings user

    {
        "user": {
            "debug": false,
            "delay": 0.2,
            "error_color": "D02000",
            "gutter_theme": "Packages/SublimeLinter/gutter-themes/Default.gutter-theme",
            "gutter_theme_excludes": [],
            "lint_mode": "background",
            "linters": {
                "csslint": {
                    "@disable": false,
                    "args": [],
                    "errors": "",
                    "excludes": [],
                    "ignore": "",
                    "warnings": ""
                },
                "flake8": {
                    "@disable": false,
                    "args": [],
                    "builtins": "",
                    "excludes": [],
                    "ignore": "E501,E128",
                    "jobs": "1",
                    "max-complexity": -1,
                    "max-line-length": null,
                    "select": "",
                    "show-code": false
                },
            },
            "mark_style": "outline",
            "no_column_highlights_line": false,
            "passive_warnings": false,
            "paths": {
                "*": [],
                "linux": [],
                "osx": [],
                "windows": []
            },
            "python_paths": {
                "linux": [],
                "osx": [],
                "windows": []
            },
            "rc_search_limit": 3,
            "shell_timeout": 10,
            "show_errors_on_save": false,
            "show_marks_in_minimap": true,
            "syntax_map": {
                "html (django)": "html",
                "html (rails)": "html",
                "html 5": "html",
                "php": "html",
                "python django": "python"
            },
            "warning_color": "DDB700",
            "wrap_find": true
        }
    }

## Step 3 - Install Linters

Linters now need to be installed using NPM (globally). The list of available linters [https://github.com/SublimeLinter](https://github.com/SublimeLinter).

Linters that should be installed (See attached URL for details on installtion process):

- Flake8 - [https://github.com/SublimeLinter/SublimeLinter-flake8](https://github.com/SublimeLinter/SublimeLinter-flake8)
- csslint - [https://github.com/SublimeLinter/SublimeLinter-csslint](https://github.com/SublimeLinter/SublimeLinter-csslint)
- eslint - [https://github.com/roadhump/SublimeLinter-eslint](https://github.com/roadhump/SublimeLinter-eslint)


## Step 4 - Install snippets

See the snippets directory for more information


## Step 5 - Enable babel syntax highlighting for ES6 + React stuff

Setting as the default syntax

To set it as the default syntax for a particular extension:

Open a file with that extension,
Select View from the menu,
Then Syntax -> Open all with current extension as... -> Babel -> JavaScript (Babel).
Repeat this for each extension (e.g.: .js and .jsx).
