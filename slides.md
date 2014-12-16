# Meet the PHPockers
Robin Speekenbrink

18 december 2014
AmsterdamPHP

<section data-markdown="slides.md" data-separator="^\n\n\n" data-vertical="^\n\n" data-notes="^Note:"></section>
---

## A brief overview of /me

@ Kingsquare

Father of 2 boys

happy-go-dev-vy

---

# Disclaimer

I just dont know and this is my first _real_ talk

Note:

 - no ops / dev care: leave the room
 - Devops 
 - Dont know 
 - Docker in flux (Rocket / 1.4)
 - CoreOS / UbuntuCore / Google / Young eco system
 - no regurgitation of docs / slides!

---

# The Talk

 - Servers - a brief history
 - Docker
 - err... PHP ?
 - Docker usage
 - Docker vs ...
 - So?
 - Awsomesauce
 - DDD
 
Note:

 - DDD Dont Do Demo's

---

# Servers - a brief history

Once upon a time...

-

# From server to droplet
 
 - Mainframes
 - Big Iron
 - Multiserver - Multitiered
 - VM's - "Droplet"
 - Vagrant
 - LXC
 - Docker

-

# ... continued

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

Note:
hard to explain, easy to use

- 

# Docker from ops (brief)

 - dont care about the inside, just the outside
 - lightweight
 - easy to manage
 - easy(ish) to scale
 - allows for faster moving applications
 - utilization limiting

Note:
stateless nodes

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

<pre><code data-trim>docker run -v $(pwd):/app -w /app php php demo/hello.php</pre>

Want to try it with PHP 5.5 ?

<pre><code data-trim>docker run -v $(pwd):/app -w /app php:5.5 php demo/hello.php</pre>

<pre><code data-trim>docker run -v $(pwd):/app -w /app php:5.6 php demo/hello.php</pre>

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
 - Spotify
 - ING
 - Kingsquare
 - Tweakers

Note:

 - Google launches 5M containers daily
 - Tweakers (partially)
 - Wercker

-

# Docker in development

 - environment vs production
 - design the image, build it and push to registry
 - PHPstorm integration
 - fig

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

-

## The future for containers
 
 - orchestration <sup>1.4</sup>
 - multi hosts <sup>1.4</sup>
 - monitoring
 - interchangeable engines (Rocket / Google)
 - Windows support
 - native Apple/Mac executor
 
-

## Docker way of life

![The docker ecosystem](/js/assets/eco.png)
(september 2014)
-

## Tech on the rise

![Metrics](/js/assets/metrics_graphic.jpg)
(december 2014)
---

# Demo time

...

Note:
 
 - see how it works for this presentation
 - dokku
 - monitoring agents 
 - mongodb 
 - memcached

---

# Links / tools etc

 - [Docker](www.docker.com)
 - [The Docker book](www.dockerbook.com)
 - [Dokku](github.com/progrium/dokku)
 - [Wercker](wercker.com)
 - [Docker Amsterdam meetup group](www.meetup.com/Docker-Amsterdam/)
 
-

## Image / data Credits
  
  - [Docker blog](http://blog.docker.com/)
  - [highscalability.com](http://highscalability.com/)
  

---

 # Fin
 
 Rate me? Ask me!
