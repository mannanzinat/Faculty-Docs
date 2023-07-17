# Introduction

[OvoyLMS](https://spagreen.net/ovoylms-learning-management-system/) is a comprehensive online learning management system designed to streamline your online education business. With a wide array of features, [OvoyLMS](https://spagreen.net/ovoylms-learning-management-system/) empowers instructors and students to connect and collaborate, fostering a vibrant knowledge-sharing environment.

Instructors using [OvoyLMS](https://spagreen.net/ovoylms-learning-management-system/) have the freedom to create an unlimited number of video courses, live classes, text-based courses, projects, quizzes, and share various files. This versatile platform allows instructors to curate educational content tailored to their expertise, enabling them to effectively impart knowledge and skills to their students.

For students, [OvoyLMS](https://spagreen.net/ovoylms-learning-management-system/) provides a rich learning experience. They gain access to a diverse range of educational materials, empowering them to enhance their skill levels and broaden their knowledge base. With [OvoyLMS](https://spagreen.net/ovoylms-learning-management-system/), students can engage with interactive course content, participate in quizzes, and explore supplementary resources.

Developed with a focus on real business needs, cultural nuances, and extensive user research, [OvoyLMS](https://spagreen.net/ovoylms-learning-management-system/) is specifically designed to meet your unique business requirements. By efficiently addressing the demands of diverse industries and learner profiles, [OvoyLMS](https://spagreen.net/ovoylms-learning-management-system/) ensures that your online education business can thrive in today's competitive landscape.

### Building Technology

- Backend Framework: PHP/Laravel 10x
- Frontend Framework:  HTML/Jquery


# Getting started

Material for MkDocs is a theme for [MkDocs], a static site generator geared
towards (technical) project documentation. If you're familiar with Python, you
can install Material for MkDocs with [`pip`][pip], the Python package manager.
If not, we recommend using [`docker`][docker].

  [MkDocs]: https://www.mkdocs.org
  [pip]: #with-pip
  [docker]: #with-docker

## Installation

### with pip <small>recommended</small> { #with-pip data-toc-label="with pip" }

Material for MkDocs is published as a [Python package] and can be installed with
`pip`, ideally by using a [virtual environment]. Open up a terminal and install
Material for MkDocs with:

=== "Latest"

    ``` sh
    pip install mkdocs-material
    ```

=== "9.x"

    ``` sh
    pip install mkdocs-material=="9.*" # (1)!
    ```

    1.  Material for MkDocs uses [semantic versioning][^1], which is why it's a
        good idea to limit upgrades to the current major version.

        This will make sure that you don't accidentally [upgrade to the next
        major version], which may include breaking changes that silently corrupt
        your site. Additionally, you can use `pip freeze` to create a lockfile,
        so builds are reproducible at all times:

        ```
        pip freeze > requirements.txt
        ```

        Now, the lockfile can be used for installation:

        ```
        pip install -r requirements.txt
        ```

  [^1]:
    Note that improvements of existing features are sometimes released as
    patch releases, like for example improved rendering of content tabs, as
    they're not considered to be new features.

This will automatically install compatible versions of all dependencies:
[MkDocs], [Markdown], [Pygments] and [Python Markdown Extensions]. Material for
MkDocs always strives to support the latest versions, so there's no need to
install those packages separately.

---

:fontawesome-brands-youtube:{ style="color: #EE0F0F" }
__[I want to learn more about OvoyLMS]__ by @james-willett – :octicons-clock-24:
15m – Learn how to create and host a documentation site using Material for 
MkDocs on GitHub Pages in a step-by-step guide.

  [I want to learn more about OvoyLMS]: https://www.youtube.com/@spagreen

---

__Tip__: If you don't have prior experience with Python, we recommend reading 
[Using Python's pip to Manage Your Projects' Dependencies], which is a really
good introduction on the mechanics of Python package management and helps you
troubleshoot if you run into errors.

  [Python package]: https://pypi.org/project/mkdocs-material/
  [virtual environment]: https://realpython.com/what-is-pip/#using-pip-in-a-python-virtual-environment
  [semantic versioning]: https://semver.org/
  [upgrade to the next major version]: upgrade.md
  [Markdown]: https://python-markdown.github.io/
  [Pygments]: https://pygments.org/
  [Python Markdown Extensions]: https://facelessuser.github.io/pymdown-extensions/
  [Using Python's pip to Manage Your Projects' Dependencies]: https://realpython.com/what-is-pip/

### with docker

The official [Docker image] is a great way to get up and running in a few
minutes, as it comes with all dependencies pre-installed. Open up a terminal
and pull the image with:

=== "Latest"

    ```
    docker pull squidfunk/mkdocs-material
    ```

=== "9.x"

    ```
    docker pull squidfunk/mkdocs-material:9
    ```

The `mkdocs` executable is provided as an entry point and `serve` is the 
default command. If you're not familiar with Docker don't worry, we have you
covered in the following sections.

The following plugins are bundled with the Docker image:

- [mkdocs-minify-plugin]
- [mkdocs-redirects]

  [Docker image]: https://hub.docker.com/r/squidfunk/mkdocs-material/
  [mkdocs-minify-plugin]: https://github.com/byrnereese/mkdocs-minify-plugin
  [mkdocs-redirects]: https://github.com/datarobot/mkdocs-redirects

??? question "How to add plugins to the Docker image?"

    Material for MkDocs only bundles selected plugins in order to keep the size
    of the official image small. If the plugin you want to use is not included, 
    create a new `Dockerfile` and extend the official Docker image:

    ``` Dockerfile
    FROM squidfunk/mkdocs-material
    RUN pip install ...
    ```

    Next, you can build the image with the following command:

    ```
    docker build -t squidfunk/mkdocs-material .
    ```

    The new image can be used exactly like the official image.

### with git

Material for MkDocs can be directly used from [GitHub] by cloning the
repository into a subfolder of your project root which might be useful if you
want to use the very latest version:

```
git clone https://github.com/squidfunk/mkdocs-material.git
```

The theme will reside in the folder `mkdocs-material/material`. After cloning
from `git`, you must install all required dependencies with:

```
pip install -e mkdocs-material
```

  [GitHub]: https://github.com/squidfunk/mkdocs-material
