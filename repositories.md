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
cares anymore)
 
### Committer: Early and active involvement
* [honeybadger-vue](https://github.com/honeybadger-io/honeybadger-vue)
* [honeybadger-react](https://github.com/honeybadger-io/honeybadger-react)

### Committer: Maintenance, active involvement
* [honeybadger-java](https://github.com/honeybadger-io/honeybadger-java)

### Contributor:
* [Semantic-UI-Vue](https://github.com/Semantic-UI-Vue/Semantic-UI-Vue)

### Purely mine
Please note that these aren't usually that interesting. In
fact, at the moment, the bulk of these are just repos for github
static pages. Maybe the probabilistic-models one is cool if
you want to see how I code in a language I didn't know very well
when I was sleeplessly dealing with being a new father 6 years ago 

{% assign filtered_repos = site.github.public_repositories | where: "fork", false | where: "archived", false %}
{% for repository in filtered_repos %}
  * [{{ repository.name }}]({{ repository.html_url }}): {{repository.description}}
{% endfor %}
