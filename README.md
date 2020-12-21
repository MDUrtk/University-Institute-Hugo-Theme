# University Institute Hugo Theme
## Install the theme

With Git installed, run the following commands inside the Hugo site folder. If Hugo has not yet been installed, read the setup guide [here](https://gohugo.io/overview/installing/).

```sh
mkdir themes
cd themes
git clone https://github.com/MDUrtk/University-Institute-Hugo-Theme.git
```

You can get a zip of the latest version of the theme from the [home page](https://github.com/MDUrtk/University-Institute-Hugo-Theme) and extract it to the themes folder.

## Update the theme

Go to the themes folder as in the installation and run the following command.

```sh
git pull
```

### config.toml
```toml
baseURL = "http://example.org/"
languageCode = "en-us"
title = "My New Hugo Site"
theme = "University-Institute-Hugo-Theme"

[[menu.main]]
name = "Home"
URL = "/"
weight = 1

[[menu.main]]
name = "Department"
hasChildren = true
weight = 2

  [[menu.main]]
  parent = "Department"
  name = "CSE"
  URL = "department/cse"
  
```

