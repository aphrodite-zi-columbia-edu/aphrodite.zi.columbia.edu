# People Templates

These layouts are being used for documents in the `_people/` directory. They
all inherit from `layout: people/people_profile`:

```
people/people_profile
├── people/postdoc_fellow
├── people/grad_student
└── people/research_other
```

These templates all require some inputs:

  * `people/people_profile`
    * `name` - string that is put on the page
    * `image` - absolute url of image (preferably in `assets/img` folder)
    * `slug` - valid url sequence to follow `//{{ site.url }}/people/`
  * `people/postdoc_fellow`
    * `degree` - string that is put on the page

The other templates are also configurable with inputs which are documented at
the top of their respective files.
