# redesign-mocks

This repository contains the redesign mocks for IMC, IRC, and Audio Dharma.

In order to view the mocks you have to build the CSS and Javascript files that the mocks depend on.

# Requirements

Working installs of modern versions of Git and Ruby are required to build the CSS and Javascript files that the mocks depend on.

# Usage

In order to view the mocks you have to build the CSS and Javascript files that the mocks depend on.

First you must install the needed dependencies. To do so run the following command from the root of the project:
```
bundle install
```

Then you can run this command to build the needed CSS and Javascript files. They will be written to the `css/` directory.

```
rake build
```

