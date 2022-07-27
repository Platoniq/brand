![Platoniq logo](./logos/Platoniq_Foundation_black_en.svg)

# The colors of Platoniq

See the full reference in [html/colors.html](./html/colors.html)

🍆 #462949
🍓 #E94668
💚 #99FF99
📄 #F3F3EF
💧 #72D8FF
💜 #B792FF
🍏 #99FFCC
🍋 #FFFF99

# Platoniq Brand in Decidim instances

To add files for custom Platoniq footer in Decidim instances, run:

```sh
chmod +x ./bin/initialize-decidim-instance-for-platoniq

./bin/initialize-decidim-instance-for-platoniq PATH_TO_DECIDIM_INSTANCE
```

To import the `platoniq.scss`, you need to add it in `app/packs/stylesheets/decidim.scss` after the `@import "decidim/application";` line, like this:

```scss
@import "decidim/application";
@import "platoniq/platoniq";
```

To overwrite the default Decidim footer with the custom one, create the file `app/views/layouts/decidim/_mini_footer.html.erb` with this content:

```erb
<%= render partial: "platoniq/mini_footer" %>
```

Finally, add the key `repository_url` to the `config/secrets.yml` with the URL of the instance's repository.

```yml
default: &default
  repository_url: https://github.com/Platoniq/decidim-INSTANCE_NAME
```

# Platoniq Brand in Decidim modules

To add files to follow Platoniq guidelines for a Decidim module, run:

```sh
chmod +x ./bin/initialize-decidim-module-for-platoniq

./bin/initialize-decidim-module-for-platoniq PATH_TO_DECIDIM_MODULE
```

To import the `platoniq.scss`, you need to add it in `app/packs/stylesheets/decidim.scss` after the `@import "decidim/application";` line, like this:

```scss
@import "decidim/application";
@import "platoniq/platoniq";
```

Finally, add the key `repository_url` to the `config/secrets.yml` with the URL of the instance's repository.

```yml
default: &default
  repository_url: https://github.com/Platoniq/decidim-INSTANCE_NAME
```

## Good Practices Checklist

### Repository

- **Naming > Repository:** If it's a Decidim __*instance*__, the repository name should be `decidim-CLIENT`
  > Replace `CLIENT` with the lowercase, hyphen-separated name of the client, ideally matching the domain name without the domain extension.
  - e.g. for city-government.org the repository name should be `decidim-city-government`

- **Naming > Repository:** If it's a Decidim __*module*__, the repository name should be `decidim-module-NAME_OF_MODULE`
  > Replace `NAME_OF_MODULE` with the lowercase, undescore-separated name of the module, matching the namespace used.
  - e.g. for `Decidim::DecidimCustomThings` the repository name should be `decidim-module-decidim_custom_things`

- **Naming > Branches:** Main branch should be named `main`, not `master`.

- **Naming > Branches:** For new features, use `feature/name-of-new-feature`
  - e.g. `feature/customize-styles`
  - e.g. `feature/restrict-access-to-space`

- **Naming > Branches:** For bugfixes, use `fix/name-of-the-bug`
  - e.g. `fix/profile-link-wrong-redirection`
  - e.g. `fix/menu-item-disappeared`

- **Naming > Branches:** For maintenance tasks (adding Github workflows, updating versions, etc.), use `chore/name-of-the-task`
  - e.g. `chore/add-lint-workflow`
  - e.g. `chore/update-to-0.25`

- **Merging:** Please delete your working branch after it has been merged to `main` (to prevent stale branches polluting the repository).