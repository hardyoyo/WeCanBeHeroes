# We Can Be Heroes

This is probably a crazy idea, but here goes:

What if we could take all the log files from a repository system, say [DSpace](https://dspace.org/),
but it doesn't have to be DSpace, it just has to be a system we load content
into, and has log files or a database that records provenance information (at
a minimum, maybe more, who knows?). We write a few quick scripts, and process
that information into files that [Gource.io](http://gource.io/) understands--[Gource has a well-
documented custom log format](https://github.com/acaudwell/Gource/wiki/Custom-Log-Format)--
and then we end up with a nice collection of videos that document, in visual form,
all the work we do to fill our repositories.

Example Gource videos:

 * [800+ days of Minecraft in 8 minutes](https://www.youtube.com/watch?v=zRjTyRly5WA)
 * [Fedora Commons development history](https://wiki.duraspace.org/download/attachments/11504727/2010-11-17-fcrepo-gource.mp4)

Think of it: the swarm of individual contributors. *Epic* batch loads. Metadata
cleanup work. We'd have a movie we could show people to visualize all the work
being done.

It gets better!

We could round up all the server log files (if we run our repository behind an
Apache HTTPD reverse proxy, or whatever we use) and run them through the similar
tool [Logstalgia](http://logstalgia.io/), and play both videos simultaneously, in a split-screen.
Then we'd be able to see the interplay of site usage and adding site content. We
all *know* adding more content brings more users. Imagine being able to *see* it?

Sound interesting? Let's make it happen.

This is going to be scrappy and messy. We'll start out with whatever works.
I have a few snippets of AWK commands that will pull data out of DSpace log files.
If this sounds like fun, make a pull request with code or just more Markdown pages
or we can just use the wiki. But, if you like this idea, let me know, I think
we can make this happen, and make it happen quickly.

# License
[BSD 3-Clause](https://opensource.org/licenses/BSD-3-Clause)
