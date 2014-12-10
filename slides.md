<section data-markdown="slides.md" data-separator="^\n\n\n" data-vertical="^\n\n" data-notes="^Note:"></section>

# Meet the PHPockers
Robin Speekenbrink

18 december 2014
AmsterdamPHP

---

## A brief overview of /me

@ Kingsquare

Father of 2 boys

happy-go-dev-vy

---

# Disclaimer

I just dont know and this is my first _real_ talk

Note: Devops / Dont know / Rocket / Docker in flux / CoreOS_UbuntuCore_Google / Young eco system

---

# The Talk

 - Servers - a brief history
 - Docker
 - err... PHP ?
 - Docker vs ...
 - So?
 - Awsomesauce

---

# Servers - a brief history

Once upon a time...

---

# From server to droplet
 
 - Mainframes
 - Big Iron
 - Multiserver - Multitiered
 - VM's - "Droplet"
 - Vagrant
 - LXC
 - Docker

![Server to docker](/js/assets/server-to-docker.jpg)

---

# Docker

Containers made easy
 = awesome!

<pre><code data-trim>docker run --rm -it ubuntu bash</pre>

-

# Docker - the essentials

virtual machines +  git + native performance = awesome = docker

 - opensource
 - OS level isolation
 - layered filesystem
 - shared kernel (cgroups)

Note: hard to explain, easy to use

- 

# Docker from ops (brief)

 - dont care about the inside, just the outside
 - lightweight
 - easy to manage
 - easy(ish) to scale
 - allows for faster moving applications
 - utilization limiting
 
- 

# Docker from dev
 
 - complete app isolation
 - better mimicing of production without the hassle
 - no more OS-differentials
 - light weight
 - easy version management of complete stack

---

# Wait, wasn't this a PHP meetup?

Yes!
Say hello to docker from a PHP standpoint

<pre><code data-trim>docker run --rm -it -v $(pwd):/myapp -w /myapp php php demo/hello.php</pre>

Want to try it with PHP 5.5 ?

<pre><code data-trim>docker run --rm -it -v $(pwd):/myapp -w /myapp php:5.5-cli php demo/hello.php</pre>

<pre><code data-trim>docker run --rm -it -v $(pwd):/myapp -w /myapp php:5.5 php demo/hello.php</pre>

- 

# Docker in action

 - easy `one-off` commands for single usecases
 - want to try the latest and greatest of PHP without reconfiguring everything?
 - why not have different FPM agents running each with various parts of your app ? (or switch languages?)
 - lean mean _clean_ development machine

---
 
# Docker in production

 - Google
 - Iron.io
 - NewRelic
 - AWS
 - Kingsquare
 - ING
 - Tweakers (?)

Note: Google launches 5M containers daily

-

# Docker in development

 - environment vs production
 - design the image, build it and push to registry
 - PHPstorm integration

-

# Docker vs ...
 
 - straight up nuthin'
 - Vagrant
 - Heroku / Appengine platforms?
 - Alternatives (Rocket / Chroot / BSD Jails / ... )

---

# Pro's and cons

-

## Con's

 - young
 - tooling
 - stability
 - infincy
 - barriers can hurt too

-

## Pro's

 - fast
 - easy
 - hipster approved
 - lightweight resource consumption
 - production ready - now

---

# Awesomesomesauce

 - easy-peasy-1-2-threezy
 - docker index
 - dokku / dokku-alt / Google / AWS
 - fig
 - young but strong!
 
---

# demo time

Note: see how it works for this presentation / dokku / monitoring agents / mongodb / memcached
Note: 

---

# links / tools etc

 - docker.com
 - [The Docker book](www.dockerbook.com/)
 - [Dokku](github.com/progrium/dokku)
 - [Wercker](wercker.com)
 - [Docker Amsterdam meetup group](www.meetup.com/Docker-Amsterdam/)
 
---

 # Fin
 
 Rate me? Ask me!
