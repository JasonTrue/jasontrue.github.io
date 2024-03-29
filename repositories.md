---
title: Jason Truesdell's Publicly-visible code
layouts: default
---

# Repositories

Most of my history is in commercial, proprietary software.
I've done lots of line-of-business application development,
web services, and even a fair bit of front-end work.
But I'm not particularly visible in the open-source world.
Here's a selection of things that I have been involved in
recently that are open-source. (I'm also a contributor to a few
other projects, but many of those are so long ago nobody
cares anymore).

### Creator
* [membrane-s3-plugin](https://github.com/YuzuTen/membrane_s3_plugin)

### Committer: Early and active involvement
* [honeybadger-vue](https://github.com/honeybadger-io/honeybadger-vue) (this is now in [honeybadger-js](https://github.com/honeybadger-io/honeybadger-js))
* [honeybadger-react](https://github.com/honeybadger-io/honeybadger-react)  (this is now in [honeybadger-js](https://github.com/honeybadger-io/honeybadger-js))

### Committer: Maintenance, active involvement
* [honeybadger-java](https://github.com/honeybadger-io/honeybadger-java)

### Contributor:
* [Semantic-UI-Vue](https://github.com/Semantic-UI-Vue/Semantic-UI-Vue)

### Purely mine

At the moment, the bulk of these are just repos for github
static pages. Maybe the probabilistic-models one is cool if
you want to see how I code in a language I didn't know very well
when I was sleeplessly dealing with being a new father 6 years ago. 

{% assign filtered_repos = site.github.public_repositories | where: "fork", false | where: "archived", false %}
{% for repository in filtered_repos %}
  * [{{ repository.name }}]({{ repository.html_url }}). {{repository.description}} {%if repository.homepage%}[(Website)]({{repository.homepage}}){%endif%}
{% endfor %}

There's also a bit of stuff on my [YuzuTen organization page](https://github.com/YuzuTen) but
it's mostly ancient (ca. 2011).

