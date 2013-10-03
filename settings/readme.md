## Sublime settings

Need to make sure all the packages listed in the initial setup doc are already installed.

#### Settings User:

	{
		"color_scheme": "Packages/Dayle Rees Color Schemes/Peacock.tmTheme",
		"font_face": "Menlo",
		"font_options":
		[
			"no_round"
		],
		"highlight_line": true,
		"tab_size": 4,
		"ignored_packages":
		[
			"Vintage"
		],
		"open_files_in_new_window": false,
		"theme": "Soda Dark.sublime-theme",
		"translate_tabs_to_spaces": true,
		"trim_trailing_white_space_on_save": true
	}

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
	    