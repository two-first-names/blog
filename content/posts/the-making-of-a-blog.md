---

title: The Making of a Blog
date: 2022-06-24
author: Joe Roberts <joe@twofirstnames.org>
draft: true

---

So I made a blog (again) and I was trying to come up with content. Then I realised “why not do a post on how you set up this post?”, so that’s where we’re at. I hope this is useful to somebody out there!

# Technologies Used

- Hugo - The site is built using Hugo[^hugo], a static site generator written in Go.
- Ansible - The blog is deployed using Ansible[^ansible], a tool used to automate deployments and commands on remote servers.
- Gitea - I’m using Gitea[^gitea] as my git server. I’ll probably do another post on how I set up Gitea and why I chose it.
- DroneCI - Everything comes together with DroneCI[^drone]. Whenever I update the blog in git, Drone deploys it using Ansible.

# Why Hugo?

There are so many static site generators out there now! Jekyll[^jekyll], Gatsby[^gatsby], Hugo[^hugo], Next.js [^nextjs], Eleventy [^eleventy]. How are you supposed to decide which one suits you?

Jekyll is probably the oldest of the bunch, written in Ruby, and has a bunch of plugins and themes. It is built for blogging from the ground up. The biggest con for me when it comes to Jekyll; it requires a full Ruby development environment to run, which can be quite daunting and a waste of resources.

Gatsby and Next.js are both React-based static site generators. This puts them apart from the others, they can be used to built a full stack website, not just a static templated markdown site. However, for what I wanted, this is a bit too much. I don’t want to mess around with React, I just want to built a site!

Eleventy is a new kid on the block, but picking up steam pretty rapidly, it is billed as a ‘simpler static site generator’. I may well try it out at some point, but for now I am going to hold my breath when it comes to ‘simple’ and ‘zero configuration’. Who knows, maybe I’ll be surprised.

Finally, and what I decided on in the end, Hugo. Hugo is written in Go (I might be a bit biased that way) and is a statically compiled binary, rather than interpreted like JavaScript or Ruby. Hugo is _fast_, and can scale to 1000s of pages in just a few seconds. The templating engine is solid, based open `html/template` and `text/template` from Go. The documentation is extensive and the community is definitely helpful. Out of the box, it supports easily making content pages, taxonomies and non-HTML (RSS, iCalendar, for example) outputs without much effort. So far I am enjoying writing with it, but since for the most part it is Markdown, I should be able to move to any other generator if I wished to.

# References

[^hugo]: https://gohugo.io/
[^ansible]: https://www.ansible.com/
[^gitea]: https://gitea.io/
[^drone]: https://www.drone.io/
[^jekyll]: https://jekyllrb.com/
[^gatsby]: https://www.gatsbyjs.com/
[^nextjs]: https://nextjs.org/
[^eleventy]: https://11ty.dev/