[![Create a Slack Account with us](
    https://img.shields.io/badge/Create_Slack_Account-The_Carpentries-071159.svg)](
        https://swc-slack-invite.herokuapp.com/)
[![Slack Status](
    https://img.shields.io/badge/Slack_Channel-dc--socsci--openref-E01563.svg)](
        https://swcarpentry.slack.com/messages/C9Y0UEXPY)
[![DOI](https://zenodo.org/badge/92422790.svg)](https://zenodo.org/badge/latestdoi/92422790)

# OpenRefine for Social Sciences

This is a Data Carpentry lesson on OpenRefine for social scientists.
Please see <https://datacarpentry.org/openrefine-socialsci/> for a rendered version of this lesson.

This is an introduction to OpenRefine designed for participants with no previous experience.
This lesson can be taught in ~ 2 hours, excluding setup.
The episodes in this lesson cover introductory topics related to using OpenRefine.

The [instructor notes][in] contain some tips about how to best teach this workshop.

## Contributing

We welcome all contributions to improve the lesson!
The [maintainers](#maintainers) will do their best to help you if you have any
questions, concerns, or experience any difficulties along the way.

We'd like to ask you to familiarize yourself with our [Contribution Guide](CONTRIBUTING.md) and
have a look at the [more detailed guidelines][lesson-example] on proper formatting, ways to render
the lesson locally, and even how to write new episodes.

Please see the current list of [issues][ghri] for ideas for contributing to this lesson.
For making your contribution, we use the [GitHub flow][github-flow].
Look for the tag ![good_first_issue](https://img.shields.io/badge/-good%20first%20issue-gold.svg).
This indicates that the maintainers will welcome a pull request fixing this issue.

### Making changes to the contents

*Please read [Contributing](CONTRIBUTING.md) before starting the work.
This section and the next are only a very brief introduction to providing changes.*

This lesson website is built from Markdown files using the Jekyll static site generator.
The episodes that make up this lesson are in the `_episodes` directory.
If you want to create a pull request (PR) with changes in any of the episodes or other Markdown
files, it helps if you can preview the results of your changes before you submit the PR.
This is explained in the next section.

The [lesson example][lesson-example] explains all the steps needed to create and update a lesson
like this one.

### Previewing the lesson on your computer

*This is helpful for submitting a pull request, but not required.*

Please see the [instructions on setting up your computer for previewing the lesson][setup].
Previewing the lesson requires Ruby and the `bundler` gem;
if you have [Make][make], the commands become shorter.

To preview any changes on your own computer, you may either:

- use [GNU Make][make]: `make serve` or `make site`; or
- use Jekyll directly:
    1. `bundle config set --local path .vendor/bundle && bundle install && bundle update`
    2. `bundle exec jekyll serve` or `bundle exec jekyll build`

The `serve` commands start a webserver that updates the output every time you save a file.
The `site`/`build` commands only create the HTML output in the `_site` directory.

See [Checking and Previewing][check] for more information on previewing your changes,
as well as commands for running various checks.

## Maintainers

The current maintainers of this lesson are:

- [Ben Companjen](https://github.com/bencomp)
- [Emilia Gan](https://github.com/efran)

They can usually be reached in our [Slack channel] and through [issues in the GitHub
repository][ghri].

[in]: https://datacarpentry.org/openrefine-socialsci/guide/
[Slack channel]: https://swcarpentry.slack.com/messages/C9Y0UEXPY
[lesson-example]: https://carpentries.github.io/lesson-example/
[ghri]: https://github.com/datacarpentry/openrefine-socialsci/issues
[github-flow]: https://guides.github.com/introduction/flow/
[setup]: https://carpentries.github.io/lesson-example/setup.html
[make]: https://www.gnu.org/software/make/
[check]: https://carpentries.github.io/lesson-example/07-checking/index.html
