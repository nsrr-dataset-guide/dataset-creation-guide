# Adding New Variables

Once you've created a basic version of your data dictionary, you're ready to add variables to it. For NSRR, all variables and domains are stored as individual JSON files, which look something like this:

    [
        "id": "variable_id",
        "display_name": "variable_name",
        "description": "A description of the variable",
        "type": "vartype",
        "units": "optional",
        "calculation": "optional",
        "domain": "optional",
        "forms": [
            "variable_form1",
            "variable_form2"
        ],
        "labels": [
            "label1",
            "label2"
        ],
        "commonly_used": true/false
    ]
Of all the modifiers above, the ones that are always required for a variable is **id**, **display_name**, **description**, and **type**. Depending on the variable type selected, **units** or a **domain** will also be required. Valid variable types are listed below:

- identifier
- choices
    - requires a domain
- integer
    - can have units or a calculation
- numeric
    - can have units or a calculation
- string
- text
- date
- time
- datetime
- file (for uploading files)

As specified above, variables that are `type: choices` require a domain. Domains lists of possible options for variables that would have pre-defined choices (like a dropdown). Domains are stored in a separate JSON file, and get referenced in the variable file.

    [
        {
            "value": "1",
            "display_name": "Option name 1",
            "description": "A description of the option"
        },
        {
            "value": "2",
            "display_name": "Option name 2",
            "description": "A description of the option"
        },
        {
            "value": "3",
            "display_name": "Option name 3",
            "description": "A description of the option"
        }
    ]
Any variable, regardless of type, can be associated with `labels` or `forms`. `Labels` are used to add additional tags to variables that are not found elsewhere in the JSON file that you would search for on [sleepdata.org](https://sleepdata.org). The `forms` field allows you to group variables together, such as variables from the same CRF, when creating a codebook. More documentation and examples of variables and domains can be found at the bottom of the Spout README on [GitHub](https://github.com/sleepepi/spout)
