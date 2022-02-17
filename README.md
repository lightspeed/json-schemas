<!-- markdownlint-disable MD033 MD041 -->
<div id="top"></div>

<!-- PROJECT LOGO -->
<br />
<h3 align="center">JSON Schemas</h3>

  <p align="center">
    Common custom JSON schemas used at Lightspeed
    <br />
    <a href="https://github.com/lightspeed/json-schemas"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/lightspeed/json-schemas/issues">Report Bug</a>
    ·
    <a href="https://github.com/lightspeed/json-schemas/issues">Request Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li><a href="#%EF%B8%8F-installation">Installation</a></li>
    <li><a href="à#-using-the-schema">Using the Schema</a></li>
    <li><a href="#-contributing">Contributing</a></li>
    <li><a href="#%EF%B8%8F-project-feedback">Project feedback</a></li>
    <li><a href="#%EF%B8%8F-license">License</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## 💁🏻‍♂️ About The Project

To faciliate writing and maintaining valid configuration files and JSON files,
we needed a way to defined the specific structure. Paired with a compatible IDE
like Visual Studio Code, we can even have inline validation.

The schema is versioned according to the [SchemaVer
technique](https://snowplowanalytics.com/blog/2014/05/13/introducing-schemaver-for-semantic-versioning-of-schemas/#schemaver)
and each version is a different file suffixed with the version using the pattern
`N-N-N`.

<!-- INSTALLATION -->
## ⚡️ Installation

Cloning the repository is enough to browse the schemas, but if you want to
contribute, we encourage you to install this validation tool which will be very
simple to use to check if the changes you provide are valid:

```bash
go install github.com/santhosh-tekuri/jsonschema/cmd/jv@latest
```

<!-- USING THE SCHEMA -->
## 📝 Using the Schema

The easiest way to leverage one of these schemas is to reference it in your JSON
or YAML file and use a compatible IDE like Visual Studio Code:

```json

```

```yaml
# yaml-language-server: $schema=https://raw.githubusercontent.com/lightspeed/json-schemas/main/schemas/repository-owners-1-0-0
```

<!-- CONTRIBUTING -->
## 🧑‍🤝‍🧑 Contributing

After understanding SchemaVer, you can add a new version file by following the
model, addition or revision pattern.

Once you are done with your new file, you can run the following command to
validate it:

```bash
jv schemas/schema-1-1-1
```

If the output is empty, the schema is valid.

<!-- PROJECT FEEDBACK -->
## ⭐️ Project feedback

If you want to say **thank you** or/and support active development of `JSON
Schema`:

- Add a [GitHub Star](https://github.com/lightspeed/json-schemas) to the
  project.
- Have a bug or a feature request? Head over to the
  [Issues](https://github.com/lightspeed/json-schemas/issues), and we will
  gladly look into this!

- Together, we can make this project **better** every day! 😘

<!-- LICENSE -->
## ⚠️ License

The MIT License (MIT) 2022 - [Lightspeed Commerce
inc.](https://lightspeedhq.com) Please have a look at the
[LICENSE](./LICENSE.md) for more details.
