![Platoniq logo](./images/platoniq-logo.svg)

# Platoniq Brand in Decidim instances

To add files for custom Platoniq footer in Decidim instances, run:

```sh
chmod +x ./bin/decidim-platoniq-brand
./bin/decidim-platoniq-brand PATH_TO_DECIDIM_INSTANCE
```

To import the `platoniq.scss`, you need to add it in `app/stylesheets/decidim.scss` after the `@import "decidim/application";` line, like this:

```scss
@import "decidim/application";
@import "platoniq/platoniq";
```

To overwrite the default Decidim footer with the custom one, create the file `app/views/layouts/decidim/_mini_footer.html.erb` with this content:

```erb
<%= render partial: "platoniq/mini_footer" %>
```