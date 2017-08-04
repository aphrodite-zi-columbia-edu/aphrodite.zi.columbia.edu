# Layouts

As of this commit, `efad06be3fd8623b2268b810d902ca55fd550032`, the layout hierarchy is:

```
document
└── has_padded_menu
    └── people/research_other
        ├── people/postdoc_fellow
        ├── people/grad_student
        └── people/research_other
```

`document` contains 

```
html
├── {% include head.html %}
└── body
    └── div.container
        └── {{ content }}
```

`{{ content }}` renders from child layouts, head.html file is documented in
`_includes/` section.

`has_padded_menu` continues, replacing the content block from above:

```
├── nav.navbar.navbar-default
└── {{ content }}
```

Thus, `people/people_profile` is the only layout to define a row:

```
{{ content }}
└── div.row
    └── div.row
        └── .col-md-3
        └── .col-md-9
            └── {{ content }}
```
