# WebsiteTemplate
### powered by [WebsiteBuilder](https://github.com/informatics-sa/WebsiteBuilder)
This is an example website showcasing the WebsiteBuilder API; Commonly used to create Saudi olympiad teams' websites, to preserve history of the olympiads in one place.

This website includes: olympiads, participations, members and contact.

## Documentation
Read Website [public data files documentation](https://sainformatics.org/data/).

You might also refer to [Developer documentation](https://sainformatics.org/data/dev).


## Local Build
### Prerequisites
You need:

- [Python Interpreter](https://python.org)
- [Ruby Interpreter](https://www.ruby-lang.org)
- Python dependencies [requests](https://pypi.org/project/requests/) and [semver](https://pypi.org/project/semver/); install using pip (or your system's python package manager):
  ```sh
  pip install requests semver
  ```
- Install Ruby dependencies using [Bundler](https://bundler.io):
  ```sh
  bundle install
  ```

<details>
    <summary>How does it work?</summary>
    `bundle` is a package manager, `Gemfile` contains the packages list.
    Jekyll latest version is 4.4.1, but the current version used in Github pages is 
</details>

### Building & Local Serving
```sh
python prebuild.py && python build.py && bundle exec jekyll serve -s ./root
```

If you have WebsiteBuilder locally you can do:
```sh
python prebuild.py --path ../WebsiteBuilder && python build.py && bundle exec jekyll serve -s ./root
```

## License
This project is licensed under the GNU General Public License v3.0.

Check [LICENSE](/LICENSE)
