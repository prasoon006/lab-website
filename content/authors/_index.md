---
cms_exclude: true

# To publish author profile pages, remove all of the `_build` and `cascade` settings below.



---


<ul>
    {{ range .Pages.ByWeight }}
        <li>
            <h1><a href="{{ .Permalink }}">{{ .Title }}</a></h1>
            <time>{{ .Date.Format "Mon, Jan 2, 2006" }}</time>
        </li>
    {{ end }}
</ul>