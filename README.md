# National Taxonomy of Exempt Entities

National Taxonomy of Exempt Entities (NTEE) codes are used by the IRS and others to classify nonprofit organizations in the United States. If you are working on a project that requires classification of nonprofit organizations, NTEE codes can be quite handy. You can learn more about NTEE codes at the [Urban Institute website][urban].

While NTEE codes are freely public, I didn't find the codes in friendly formats. This project provides NTEE codes, titles, descriptions, and keywords in a JSON file.

I pulled the NTEE codes, titles, descriptions, and keywords from the [National Center for Charitable Statistics NTEE search page][search].

## JSON structure

Each NTEE code is a top level key, with the value a dictionary of the following three attributes:

- <code>title</code>: A plain language title for the NTEE code
- <code>description</code>: Description for the NTEE code
- <code>keywords</code>: A list of strings where each string is a keyword

```javascript
{
    "ntee_taxonomy_code" : {
        "title" : "title",
        "description" : "description",
        "keywords": [
            "keyword_1",
            "keywords_2"
        ]
    }
}
```

[urban]: http://nccs.urban.org/classification/NTEE.cfm
[search]: http://www.nccsdataweb.urban.org/PubApps/nteeSearch.php?gQry=all&codeType=NTEE