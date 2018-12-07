# Sublime setup

This Repo contains some useful help on getting a fresh install of Sublime Text setup.

## Step 1 - Install package manager

First you need to install the sublime package controller which you can get from [https://sublime.wbond.net/](https://sublime.wbond.net/).

When this is done it should be relatively simple to install the following packages by pressing `CMD` + `SHIFT` + `P` and typing `install package`.

#### Installed Packages:

    "Dayle Rees Color Schemes",
    "SideBarEnhancements",
    "SublimeLinter",
    "MarkdownEditing",
    "Theme - Soda",
    "Theme - Spacegray",
    "Babel",
    "GitGutter",
    "MagicPython",
    "TOML",
    "Dockerfile Syntax Highlighting"


## Step 2 - Sublime settings

After you have installed all the packages you can add in your preferences -> settings - user

#### Settings User:

```
{
    "color_scheme": "Packages/User/base16-ocean.dark (SL) (Flake8Lint).tmTheme",
    "font_face": "Menlo",
    "font_options":
    [
        "no_round"
    ],
    "font_size": 14.0,
    "highlight_line": true,
    "ignored_packages":
    [
        "Markdown",
        "Vintage"
    ],
    "open_files_in_new_window": false,
    "tab_size": 4,
    "theme": "Spacegray.sublime-theme",
    "translate_tabs_to_spaces": true,
    "trim_trailing_white_space_on_save": true
}
```


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

```
{
    "rulers": [100],
    "tab_size": 2,
    "extensions":
    [
        "js"
    ]
}
```



#### Sublime linter settings user

```
{
    "debug": false,
    "delay": 0.25,
    "lint_mode": "background",
    //"gutter_theme": "Packages/SublimeLinter/gutter-themes/Blueberry/cross/Blueberry - cross.gutter-theme",
    "gutter_theme": "Default",
    "styles": [{
        "mark_style": "outline",
        "priority": 1,
        "scope": "sublimelinter.mark.warning",
        "icon": "triangle",
        "types": [
            "warning"
        ]
    }, {
        "mark_style": "fill",
        "priority": 0,
        "scope": "sublimelinter.mark.error",
        "icon": "x",
        "types": [
            "error"
        ]
    }],
    "linters": {
        "eslint": {
            "@disable": false,
            "args": [],
            "excludes": [],
            "env": {"PATH":"/usr/local/bin/"}
        },
        "flake8": {
            "executable": "/usr/local/bin/flake8",
            "@disable": false,
            "args": [
                "--ignore=E501,E512"
            ],
            "builtins": "",
            "ecmaFeatures": {
                "jsx": true,
                "modules": true
            },
            "excludes": [],
            "ignore_match": [
                "E501",
                "E512"
            ],
            "jobs": "1",
            "max-complexity": 8,
            "max-line-length": null,
            "select": "",
            "show-code": false
        },
        "pylint": {
            "executable": "/usr/local/bin/pylint",
            "args": [],
            "excludes": [],
            "ignore_match": [
                "D100",
            ],
            "rcfile": "",
            "show-codes": false
        }
    },
    "no_column_highlights_line": false,
    "show_marks_in_minimap": true,
    "syntax_map": {
        "html (django)": "html",
        "html (rails)": "html",
        "html 5": "html",
        "javascript (babel)": "javascript",
        "magicpython": "python",
        "php": "html",
        "python django": "python",
        "pythonimproved": "python"
    }
}
```

## Step 3 - Install Linters

Linters now need to be installed using NPM (globally). The list of available linters [https://github.com/SublimeLinter](https://github.com/SublimeLinter).

Linters that should be installed (See attached URL for details on installtion process):

- Flake8 - [https://github.com/SublimeLinter/SublimeLinter-flake8](https://github.com/SublimeLinter/SublimeLinter-flake8)
- PyFlakes - [https://github.com/SublimeLinter/SublimeLinter-pyflakes](https://github.com/SublimeLinter/SublimeLinter-pyflakes)
- csslint - [https://github.com/SublimeLinter/SublimeLinter-csslint](https://github.com/SublimeLinter/SublimeLinter-csslint)
- eslint - [https://github.com/roadhump/SublimeLinter-eslint](https://github.com/roadhump/SublimeLinter-eslint)

Dont forget to install flake8 and pyflakes for Python 3:

	sudo pip3 install flake8 --upgrade
	sudo pip3 install pyflakes --upgrade
    sudo pip3 install mccabe --upgrade


## Step 4 - Install snippets

See the snippets directory for more information


## Step 5 - Enable babel syntax highlighting for ES6 + React stuff

Setting as the default syntax

To set it as the default syntax for a particular extension:

Open a file with that extension,
Select View from the menu,
Then Syntax -> Open all with current extension as... -> Babel -> JavaScript (Babel).
Repeat this for each extension (e.g.: .js and .jsx).
