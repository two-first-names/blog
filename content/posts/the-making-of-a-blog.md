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

# References

[^hugo]: https://gohugo.io/
[^ansible]: https://www.ansible.com/
[^gitea]: https://gitea.io/
[^drone]: https://www.drone.io/