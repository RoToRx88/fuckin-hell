# Fu*kin' hell

* Safari doesn't support the port `8090` for localhost debug
    * Browserstack, safari, ios, apple, port, npm
    * __FIX:__ change port in `package.json` to `5757` instead of `8090`
    * [reference](https://www.browserstack.com/question/664)
* Angular4 to declare directive use the `@Directive({selector: '[]'})`
    * Angular4, directive, declaration, component
    * [reference](https://angular.io/guide/attribute-directives)
* Git push not working after rebase (simple or with merge conflict): --force is required
    * git, rebase, push, force, conflict, merge
* Access profile list in terminator
    * Alt+L then select a profile with arrows then Enter
* JSON model generator from JSON file
    * https://app.quicktype.io/
* `npm link` to link local modules together
    * https://medium.com/trisfera/the-magic-behind-npm-link-d94dcb3a81af
* crontab useful list
    * https://tecadmin.net/crontab-in-linux-with-20-examples-of-cron-schedule/
* crontab that are useful and intuitive
    * @daily @weekly @monthly...
* Mobile scroll laggy lag, javascript handler
    * https://github.com/WICG/EventListenerOptions/blob/gh-pages/explainer.md
* `tig` to checkout a branch
    * https://www.atlassian.com/blog/git/git-tig
    * `tig --all`
    * r
    * select the branch you want to checkout
    * C
    * y
    * you're on the branch you want
* Firefox not working with vuejs
    * `dom.webcomponents.customelements.enabled` in `about:config` needs to be at `true`
* oneko
    * Litlle cat that follow your mouse
* AngularJS pass variable from html to js in directive like `<myDirective myvar="value">`
    * In JS the binding can be done with many params 
        * http://blog.krawaller.se/posts/dissecting-bindings-in-angularjs/
    * When using camelCase, in js to: camelCase and in html do camel-case
        * Yes it will bind the data even if the two variables have not the exact same name
* Linux create user without home dir
    * `useradd` to create withOUT home dir _(native binary)_
    * `adduser` to create WITH home dir _(perl script more userfriendly)_
* Nginx refuse file over 1Mo
    * ` client_max_body_size 0;`
* Git push from a repo to an other on forked from the first
    * https://stackoverflow.com/questions/25545613/how-can-i-push-to-my-fork-from-a-clone-of-the-original-repo
* Test de charge, load, testing
    * https://access.redhat.com/documentation/en-us/red_hat_satellite/6.2/html-single/hammer_cli_guide/index
* `tee` command in linux
    * Act like a T pipe in a pipeline so one can catch the flow in the pipe to route it in a file
    * https://stackoverflow.com/questions/764463/unix-confusing-use-of-the-tee-command
* JSON processor, parser, stream, pipe, sorting
    * `jq`
    * _example:_ `curl "https://ip-ranges.amazonaws.com/ip-ranges.json" | jq '.prefixes[] | select(.region == "us-east-1") | .ip_prefix'`
    * https://shapeshed.com/jq-json/
* ssh execute script when connection detected
    * https://askubuntu.com/a/448602
    * `/etc/pam.d`
    * `session optional pam_exec.so seteuid /etc/ssh/oth.sh`
* Good documentation on `sed`
    * http://www.grymoire.com/Unix/Sed.html#uh-0
* bash, condition, if, statment
    * bash seams to interprate the if statment an other way
    * if 0; will go in the if
    * if 1; will skip the if block
* tmux, synchronize, broadcast, pan
    * send keyboard input to multiple pan of tmux
    * `Ctrl-B :`
    * `setw synchronize-panes on`
* acl, permissions, access
    * token is associated to acl so when creating a new acl __sometimes we need to empty the browser cache and reconnect to create a new token__
* mongodb, engodage, document, utf-8
    * Mongodb BSON can only be encoded in UTF-8
    * src: https://stackoverflow.com/questions/14356652/how-to-set-mongodb-charset-to-utf8
* css, transition, smooth
    * `transition-duration: 0.5s`
* rename, linux, command, batch, perl, regex
    * sudo apt install rename -y
    * Command that allow renaming file with perl regex style matching
* linux, ssh, key, rsa, email, comment
    * The email / host written at the end of the public key is only for comment purpose and have no impact whatsoever on the key itself
    * https://serverfault.com/questions/309171/possible-to-change-email-address-in-keypair
* typescript, angular, interface, nodejs, class
    * If needs to cast an object to a part only of an interface
    * `Partial<myIface>`
* typescript, javascript, enum, class, numeral to string
    * If required to access string value of an enum do as so
    * myEnumClass[myenumValue] => string
* tmux, zoom, pane, scale
    * To zoom in and out of a tmux pane, just `prefix-z`
* ubuntu, linux, reset, password, root, emergency, boot
    * init=/bin/sh
    * mount -o remount,rw /
    * passwd username
    * https://askubuntu.com/questions/24006/how-do-i-reset-a-lost-administrative-password
* docker, container, reatart, boot, reboot
    * `docker update --restart=no my-container`
    * to prevent a container of restarting automatically at boot time of the computer
* linux, ssh, X, display
    * https://unix.stackexchange.com/questions/10121/open-a-window-on-a-remote-x-display-why-cannot-open-display?newreg=6d3790fc26b744379e51171e4e163d2b
    * export DISPLAY=:0
    * check if the XAUTHORITY is set and set it with the .Xauthority file usually under ~
* reload, tmux, config
    * C-: `:source-file ~/.tmux.conf`
    * https://sanctum.geek.nz/arabesque/reloading-tmux-config/
* shell, check, moulinette
    * To check validity of a shell script
    * https://www.shellcheck.net/#
* http proxy, monitor, reverse proxy, https
    * https://www.charlesproxy.com/
    * To analyse network and requests send by an application on a computer
* (OTHER, FUN, DATA, FAKE, SPURIOUS, CORRELATION)
    * http://www.tylervigen.com/spurious-correlations 
* remove, background, image, png, automatic
    * https://www.remove.bg/
* truth table, javascript, ==, ===
    * https://dorey.github.io/JavaScript-Equality-Table/
* javascript, paser, bullshit
    * https://charlieharvey.org.uk/page/javascript_the_weird_parts
* linux, swap, management, ram
    * linux by default swap when RAM is around 50%
    * https://askubuntu.com/questions/103915/how-do-i-configure-swappiness
    * https://unix.stackexchange.com/questions/88693/why-is-swappiness-set-to-60-by-default
* speed, dd, linux
    * `status=progress`
* shell, over, roaming, linux, ssh, data
    * https://github.com/mobile-shell/mosh
    * Shell that allows roaming for ssh connections
* vim, paste, mode
    * https://askubuntu.com/questions/256782/how-to-copy-paste-contents-in-the-vi-editor
    * `:set paste` then paste the content
    * `:set nopaste` to return to normal mode
* text, file, carriage, return, new line, linux, dos, unix
    * `od -dc myFile`
    * Allow to show if there is only a `\n` or if there is a `\r\n` in the file
    * https://www.networkworld.com/article/3107972/windows-vs-unix-those-pesky-line-terminators.html
* squash, merge, git, feature
    * `git merge --squash feature/xx + commit` proposed by Victor B. to merge a branch and squashing all the commits
* console, dev, tools, devtools, chrome, f12
    * A lot of great tricks helping with google's dev tool
    * https://medium.com/frontmen/art-of-debugging-with-chrome-devtools-ab7b5fd8e0b4
* curl, proxy, prevent, direct, connection
    * `curl --noproxy '*' myurl.com`
    * Allow one to reach a url without using a proxy if one is configured
* javascript, replace, switch
    * use map {}
* git, bisect, dichotomy, bug, find, commit, responsible
    * https://git-scm.com/book/en/v2/Git-Tools-Debugging-with-Git
    * `git bisect`
    * Helps one to find which commit introduced a bug
* git, log, search, branch, info, regex, find, grep
    * To search for a string / regex in git history
    * `git log --all --grep='string to search'`
* rm, alternative, unlink, posix, C library
    * To remove a file on UNIX systems `rm` is usually used but another one exists: `unlink`
    * The following is a good explanation of why `unlink` can be better than `rm` sometimes
    * https://unix.stackexchange.com/a/326711/332637
* trace, system, call, syscall, linux, command, shell
    * To see what a command does in depth the use of `strace` helps to see all system call performed
    * `man strace`
* zip, gzip, tar, compression, knowledge
    * Nice article about zip file type + differences with tar etc...
    * https://stackoverflow.com/questions/20762094/how-are-zlib-gzip-and-zip-related-what-do-they-have-in-common-and-how-are-they
* git, rebase, vs, merge
    * Good explenation of why git sometimes wants to merge origin onto the local branch
    * https://stackoverflow.com/questions/8509396/git-pull-results-in-extraneous-merge-branch-messages-in-commit-log
* git, graph, decision, making
    * When you screw your git and want to know how to fix it
    * [link](https://camo.githubusercontent.com/e7fa6323f06a0e9a3f59fc8c0202f1d005c7bccd/687474703a2f2f6a757374696e68696c656d616e2e696e666f2f61727469636c652f6769742d7072657474792f6769742d7072657474792e706e67)
* unlock, whitepaper, white, paper, crack, science, hub, free
    * https://sci-hub.se/
* ebook, epub, free, crack, book
    * http://libgen.io/
* get, current, git, branch, name
    * `git rev-parse --abbrev-ref HEAD`
    * https://stackoverflow.com/a/12142066/10036615
* nodejs, js, javascript, node, angular, ES6, ecmascript6 import, require, from
    * `const toto = require('toto')`
    * in ES6 can be translated by
    * `import * as toto from 'toto'`
    * https://stackoverflow.com/a/41179861/10036615
* jira, search, JQL, advanced, update, timeframe,
    * To find a ticket that has been updated to a specific status in a defined timeframe
    * `status changed to <yourStatus> DURING ("2019/05/01 00:00","2019/05/13")`
* computer, science, laws, adage
    * https://github.com/dwmkerr/hacker-laws#conways-law
* linux, cmd, command, line, size, disk, full, free, available, space
    * ncdu
* vim, json, format, object
    * `:%!python -m json.tool`
    * https://blog.realnitro.be/2010/12/20/format-json-in-vim-using-pythons-jsontool-module/
* vim, move, line
    * `:m+12` moves the current line 12 lines down
* zenity, linux, tool, notification, pop-up, warning
    * `man zenity`
* linux, mouse, trackpad, scrolling, i3wm
    * `xinput set-prop <mouse_id> <mouse_property> 1`
    * to get mouse_id: `xinput list`
    * then to get the mouse_property: `xinput list-props <mouse_id>`
* secret, management, ops, linux, password
    * https://www.vaultproject.io/
* linux, rename, files, regex, perl
    * To rename many files at once with a regex
    * `rename s/patternToSearch/replacement/g *.myfiles`
* linux, i3, bar, status, i3bar
    * barista
    * https://barista.run/#quickstart
* ubuntu, linux, apt, apt-get, aptitude, unmet, dependencies, install
    * If running into the error "unmet dependencies" while installing a soft on ubuntu
    * use `aptitude` and say NO to the first proposition, the next one will solve most of the time the issue
* linux, ssh, disconnect, connected, person
    * `who -u` get the pid then `kill`
* linux, ssh, write, tty
    * `echo 'Hello World' | write <user> pts/x`
* vim, macro, repeat
    * souce: https://vim.fandom.com/wiki/Macros
    * `q` trigger the macro system
    * `anyLetter` to save the macro on a letter
    * Anything you want to do in the macro
    * `q` to finish the record
    * `@anyletter` to play the macro
* search, ag, grep, ack,
    * Search but much faster: `ag`
* docker, enter, container, exec, root
    * To enter a container as root do `docker exec -u 0 -it /bin/bash`
* docker, compose, container, ping, local
    * To reach a container from another one in a docker-compose, we can use it's name in the docker-compose as hostname
    * if we have two containers `elasticsearch` and `kibana` from `elasticserach` we can for instance do
    * `ping kibana` or `curl http://kibana:9200`
* linux, invert, cap lock, escape
    * `echo "setxkbmap -option caps:swapescape" >> ~/.xinitrc`
* flameshot, screenshot, linux, selection
    * flameshot = good screenshot tool w/ modification posibilities
    * https://github.com/lupoDharkael/flameshot
* nginx, internet, explorer, IE, cache
    * Prevent IE cache on nginx side
    * This goes into the `server {}` block
    * `add_header Pragma no-cache;`
    * `add_header Expires -1;`
* vim, spell, check
    * `:set nospell`
    * `:set spell`
* git, revert, merge, -m
    * https://raw.githubusercontent.com/git/git/master/Documentation/howto/revert-a-faulty-merge.txt
    * `git revert <sha1> -m 1`
        * `-m 1` is to define which parent history is the reference point
* nginx, angular, error, stream, net::ERR_INCOMPLETE_CHUNKED_ENCODING, encoding, chunk
    * When streams are too big nginx write'em down on the FS
    * If no space is left under `/var/lib/....` then it can't stream everyting and it breaks
* ag, ack, search, recursive, sack
   * `sack` is a mix of `ag` and `ack`
   * allows one to edit a file after search results came in
   * `F <indexOfResult>` and it opens the particular file
   * https://github.com/sampson-chen/sack
* data, storytelling, show, graph, visualisation
   * https://www.chartr.co/
* bash, basics, braces, brackets
  * https://stackoverflow.com/questions/2188199/how-to-use-double-or-single-brackets-parentheses-curly-braces
- vim, shell, fact, knowledge
  - Most shell don't recognise the difference between lowercase ctrl and capital ctrl
  - Thus, C-O and C-o are the same
  - source: comment of this answer: https://stackoverflow.com/a/3985410
- vim, highlight, search
  - To remove until the next search the highlighting in vim
  - `:noh`
  - WARNING: This does NOT remove the search buffer, therefore hitting `N` or `n` will cycle through the search results.
  - https://vi.stackexchange.com/questions/184/how-can-i-clear-word-highlighting-in-the-current-document-e-g-such-as-after-se
- file, parcing, csv, grep
  - `csvgrep`
  - example: `csvgrep -c 2 -m "foobar" data.csv > data_filtered.csv`
  - https://github.com/wireservice/csvkit
- package, json, angular, nodejs, script, add, npm, yarn
  - To add dynamically a script to your package.json
  - `npm-add-script`
  - https://www.npmjs.com/package/npm-add-script
- linux, cli, disk, analyser, space, size
  - `ncdu`
- teamviewer, control, remote, desktop
  - https://parsecgaming.com/
- nginx, htpasswd, basic, auth, basicauth
  - Generate encrypted password `perl -le 'print crypt("your-password", "salt-hash")'`
  - Create `.htpasswd` file containing `user:encryptedPassword`
  - Setup conf in nginx location block
   - `auth_basic "Administrator Login";`
   - `auth_basic_user_file /path/to/.htpasswd;`
- wireguard, vpn, setup, tutorial
  - https://grh.am/2018/wireguard-setup-guide-for-ios/
- xresources, reload, file
  - `xrdb -load ~/.Xresources`
- vim, escape, sequence, theme, color, scheme, reset, fuck, shell
  - Vim sends an escape sequence to the terminal upon exit to reset the color scheme
  - https://vi.stackexchange.com/questions/11911/how-can-vim-be-configured-to-restore-normal-terminal-color-on-exit
- git, following, file, assume, unchanged, difference
  - There is two ways to stop following a file and keep it in the tree, here is an explanation of the diff
  - https://stackoverflow.com/questions/13630849/git-difference-between-assume-unchanged-and-skip-worktree#
  - TL;DR
    - use `git update-index --skip-worktree [FILE]` unless for performance issues calling stat
- lock, mutex, shelll, linux
  - `flock` allows us to use a lock mechanism at systemwise
  - `fuser` to gather information abfout a lock file
- ubuntu, cron, folder, cron.daily,
  - on ubuntu there is many folder `/etc/cron.{hourly,daily,weekly,monthly}` where we can direcly put custom crontab files
- bastion, ssh, key, forward, multiple, machine, ssh
  - `ssh -A` used to forward key stored in the current ssh-agent
  - `ssh user@finalHost -J user@bastion` allows to use a bastion as a jump platform for ssh
- number, human, contact, relationship, limit, dunbar
  - https://www.wikiwand.com/en/Dunbar%27s_number
- spotify, model, mgmt, agile
  - https://blog.crisp.se/wp-content/uploads/2012/11/SpotifyScaling.pdf
- network, test, service, reachable, nc, tcp
  - `nc -vz myHost myPort`
  - `nc -l -p 4242` to open a server on this port
- temp, file, tmp, create, folder
  - `mktemp` - create a temporary file or directory
- basename, file, name, directory, strip, path
  - `basename` - strip directory and suffix from filenames
- ansible, include, import, tasks, vs
  - `import_tasks` when importing at pre-processing
  - `include_tasks` on runtime so dynamic
  - https://serverfault.com/questions/875247/whats-the-difference-between-include-tasks-and-import-tasks
- vim, snippets, UltiSnips
  - dependant of filetype
  - https://github.com/SirVer/ultisnips
- bash, pipe, redirection, fd, file, descriptor
  - great tutorial on 2>&1 etc
  - https://wiki.bash-hackers.org/howto/redirection_tutorial
- vim, registers
  - https://www.brianstorti.com/vim-registers/
- linux, cli, file, manager
  - `nnn`
- linux, image, cli
  - `catimg`
- linux, man, command, examples
  - `tldr`
- linux, gui, disk, space
  - `filelight`
- linux, antivirus, scan
  - `clamav
  - https://www.clamav.net/
- hosts, linux, network, adblock, ad, malware
  - block all domains that contains ad and all that crap
  - https://github.com/StevenBlack/hosts
- remember, flashcards, opensource, crossdevice
  - anki
  - https://apps.ankiweb.net/
- docker. cli, manager, monitor, interface
  - `lazydocker`
  - https://github.com/jesseduffield/lazydocker
- search, google, engine, cli
  - `googler` to get google search results and select to open into a browser
- convert, documents, pdf, md, markdown
  - `pandoc`
- cli, shell, background, command, nohup, no, hangup
  - `nohup <commandToExecute>` creates a `nohup.out` file and runs the command in background
- ansible, ssh, break, ctrl-c, ^c, playbook, not, working
  - sometimes when ^C while playing a playbook, when you want to start back this playbook it won't gather facts and will stay stuck. Just `pkill ssh` and trigger again the playbook
- terraform, about, configuration, management
  - > For configuration management, you should use Terraform provisioning to invoke a real configuration management solution.
  - https://learn.hashicorp.com/terraform/getting-started/provision#running-provisioners
- ansible, systemctl, --user, no, password
  - export env var `XDG_RUNTIME_DIR` when having to do ansible task `systemctl --user`
- idempotence
  - >  is the property of certain operations in mathematics and computer science whereby they can be applied multiple times without changing the result beyond the initial application.
- curl, http, code, status, response
  - curl to get only the status code
  - `curl -s -o /dev/null -w "%{http_code}" myUrl`
- ping, alternative, stats
  - `mtr`
- aws, zone, availability, region
  - A region is divided by availability zones
  - `eu-west-1{a,b,c}` where `{a,b,c}` represent each a different AZ of the region
    - each AZ is different from one AWS account to another
  > An Availability Zone is represented by a Region code followed by a letter identifier; for example, us-east-1a. To ensure that resources are distributed across the Availability Zones for a Region, we independently map Availability Zones to names for each AWS account. For example, the Availability Zone us-east-1a for your AWS account might not be the same location as us-east-1a for another AWS account.
- expose, local, port, wan
  - https://ngrok.com/
  - https://github.com/localtunnel/localtunnel
  - https://serveo.net/#self-host
- niceness, priority, running, linux, unix, kernel
  - `man nice`
- gitops, observability
  - https://www.weave.works/technologies/gitops/
  - https://www.weave.works/blog/weaveworks-gitops-developer-toolkit-part-one-skaffold
  - https://www.weave.works/blog/the-gitops-pipeline
  - https://www.weave.works/blog/gitops-part-3-observability
  - https://www.weave.works/blog/gitops-compliance-and-secure-cicd
  - https://www.weave.works/blog/gitops-operations-by-pull-request
  - https://www.weave.works/blog/kubernetes-anti-patterns-let-s-do-gitops-not-ciops
  - > Declarative means that configuration is guaranteed by a set of facts instead of by a set of instructions
- terraform, state, 404, error, bucket
  - `rm -rf .terraform` when switching backend bucket for state storage
  - then `terraform init`
- terraform, debug, crash, interpret, log
  - search for the `panic` line
  - [link](https://github.com/hashicorp/terraform/pull/5726/commits/209b69197179ac427981c64f1d89e21d43a542d7)
- cli, linux, shared, objects, librairies
  - `ldd myBin`
- arduino, vim, plugin, cli, upload, sketch
  - if permissions denied to access upload port on arduino, just add user to `uucp` group that manage every RS-232 port and devices
- unknown, linux, distribution, name, release
  - `cat /etc/*release`
- git, stash, drop, lost
  - `git log --graph --oneline --decorate $( git fsck --no-reflog | awk '/dangling commit/ {print $3}' )
  - gist source: https://gist.github.com/joseluisq/7f0f1402f05c45bac10814a9e38f81bf`
- apache, basicAuth, htpasswd, conf, vhost
  - `    <Directory "/var/www/html">
        AuthType Basic
        AuthName "Restricted Content"
        AuthUserFile /etc/apache2/.htpasswd
        Require valid-user
    </Directory>`
  - `htpasswd -c myVhost.htpasswd username`
- domain, name, dns
  - when looking for a server to connect and I only have a DNS record, use `dig` to get the associated records
- sed, serach, replace, negative lookbehind
  - `s/(?<!minimalsetup)(ssh_deployment_enabled)/minimalsetup_\1/g`
- vim, nerdTree, edit, name, file, rename
  - Renaming a file with nerdTree in vim
  - `m` then select `move` then rename
- php, debug, infos, config
  - `<?php phpinfo();`
- grub, fstab, mount, boot, error
  - `defaults,nofail`
  - > If you ever boot your instance without this volume attached (for example, after moving the volume to another instance), the nofail mount option enables the instance to boot even if there are errors mounting the volume. Debian derivatives, including Ubuntu versions earlier than 16.04, must also add the nobootwait mount option.
- deployment, capistrano, exclude, dir, not, all
  - to exclude the `build` dirs but not the one generated on ./
  - `set :exclude_dir, ['./build']` instead of `['build']`
- unmount, umount, busy, device
  - `lsof | grep <mountPoint>`
  - `kill <pidOfProcessUsingMountPoint>`
  - [more on that](https://stackoverflow.com/a/58121313)
- bash, expend, arguments, previous, command, builtin
  - `myCommand !*`
  - can use `alt+.` to cycle through arguments' history
  - [reference](https://stackoverflow.com/a/36654936)
- bash, source, config, global, system, unix
  - `/etc/profile.d/MyScript.sh` ran by all users when instanciating a shell
- zip, unzip, show, content, archive
  - `less myArchive.zip`
  - `less` is capable of showing the content of a zipfile
- apg, password, random, generator, linux, command
  - `apg` linux command to generate random passwords
- ansible, testing, molecule, docker, driver
  - to use docker as a driver for molecule
  - `pip install 'molecule[docker]'`
- vim, tutorial, learning, cli
  - `vimtutor`
- cli, linux, tutorial, learning, shell, man
  - `man man`
  - `man -a intro`
- mysql, database, size
  - `du -hs /var/lib/mysql/MyDatabaseName`
- python, local, server, fileserver
  - `python -m http.server 8000`
  - will serve the current folder it's ran in
- docker, access, host, ip, domain, dns, network
  - `host.docker.internal`
- postfix, email, error, denied, relay
  - it can be caused by the postfix server not allowed to send emails coming from a requester's foreign IP address
  - [link](https://serverfault.com/questions/775415/postfix-noqueue-reject-rcpt-from-unknown)
- google, chrome, unsafe, website, ssl, error, certificate,
  - somewhere in the grey area click, and then type `thisisunsafe`
  - `chrome://flags/#allow-insecure-localhost` and enable
  - [link](https://www.technipages.com/google-chrome-bypass-your-connection-is-not-private-message)
- mysqldump, permission, database
  - `mysqldump: Error: 'Access denied; you need (at least one of) the PROCESS privilege(s) for this operation' when trying to dump tablespaces`
  - solution: `mysqldump --user user --no-tablespaces --password dbname > myexport.sql`
  - [source](https://dba.stackexchange.com/a/273040)
- apache, allow, specific, user, agent
  - ```        
        <Proxy *>
                <RequireAny>
                        Require valid-user
                        Require env ExternalAllowed
                        SetEnvIf User-Agent "yourUserAgentHere" ExternalAllowed
                </RequireAny>
        </Proxy>
    ```

- mysql, database, processlist, request, in progress
  - `show processlist;`
  - list all requests in progress / waiting
- elk, kibana, elastic, indexation, multifields
  - When in kibana a test field has a `multi fields` status [here is the reason](https://www.elastic.co/guide/en/elasticsearch/client/net-api/current/multi-fields.html#_default_mapping_for_string_properties)
- bash, file descriptor, fd, getLine
  - [here](https://stackoverflow.com/questions/39200664/how-to-continually-process-last-lines-of-two-files-when-the-files-change-randoml)
  - `exec 3<myfile` then `read -u 3 myNewLine && myLine="${myNewLine}"`
- tail, logfile, follow, new, creation, file
  - `tail -F` will try to open a newly created file
  - `man tail`
- linux, pacman, yay, downgrade, package
  - cache under `/var/cache/pacman/pkg` run wanted package with `pacman -U`
  - [here](https://unix.stackexchange.com/questions/103859/arch-linux-pacman-specifying-package-version)
- systemctl, user, process, permission, denied
  - `export XDG_RUNTIME_DIR=/run/user/$(id -u)`
- ssh, new server, yes, type, key
  - To automatically type `yes` upon new ssh connection: `StrictHostKeyChecking no`
  - Still throw a warrning if ssh key changed
- aws, S3, fullacess, only, one, bucket
  - ```{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Effect": "Allow",
            "Action": [
                "s3:*",
                "s3-object-lambda:*"
            ],
            "Resource": [
                "arn:aws:s3:::vault-storage-production",
                "arn:aws:s3:::vault-storage-production/*"
            ]
        },
        {
            "Effect": "Allow",
            "Action": [
                "s3:ListAllMyBuckets"
            ],
            "Resource": [
                "*"
            ]
        }
    ]
}```

- vault, hashicorp, password, cli, tool, manager
  - https://github.com/fishi0x01/vsh
- gitlab, ci, skip, outdated, jobs
  - [here](https://docs.gitlab.com/ee/ci/pipelines/settings.html#skip-outdated-deployment-jobs)
- log, since, last, reboot, linux, journalctl
  - `journalctl -b -1`
- dns, history, check
  - [dnsdumpster](https://dnsdumpster.com/)
- pfx, certificate, ssl, conversion
  - `# openssl pkcs12 -in filename.pfx -out cert.pem -nodes`
  - source: [here](https://www.xolphin.com/support/Certificate_conversions/Convert_pfx_file_to_pem_file)
- varnish,detailed, logs,
  - `varnishlog -q "RespStatus >= 500 or BerespStatus >= 500"`
- apache, web, curl, local, testing, bypass, varnish
  - `curl http://localhost:80 -H 'Host: __VHOST_NAME__' -H 'X-Forwarded-Proto: https' -H 'X-Forwarded-Port: 443' -H 'X-Forwarded-For: __DESTINATION_IP__'`
- helm, range, loop, iteration, var, scope
  - when in a `range` statement the scope of `.` changes to the `range`
  - to reference our global values: `$.`
  - [ref](https://github.com/helm/helm/issues/10454)
- bash, argument, parcing, cli
  - [ref](https://stackoverflow.com/questions/192249/how-do-i-parse-command-line-arguments-in-bash)
- ntp, date, time, set, linux
  - `timedatectl`
- linux, bspwm, cursor, size
  - .config/gtk3 settings.ini
  - ~/.gtkrc-2.0
  - set the cursor size to non zero number
- rsync, non, root, user, root, stuff
  - when usually doing `ssh ubuntu@IP` then `sudo -i`
  - `rsync -avP -e "ssh" --rsync-path="sudo rsync" ubuntu@`
  - https://superuser.com/a/889313
- generate self signed testing certificates
  - `openssl req -new -newkey rsa:2048 -days 365 -nodes -x509 -keyout "${1}.key" -out "${1}.crt" -subj "/C=BE/ST=Antwerp/L=Brasschaat/O=Inuits/CN=${1}" -addext "subjectAltName = DNS:${1}"`
- dd, burn, iso, faster, pv
  - `pv < /input/file > /output/device`
  - [source](https://askubuntu.com/a/523043)
- mysql, create, user, copypaste
  - `create user '<user>'@'localhost' identified with mysql_native_password by '<mypwd>';`
  - `create database <db_name>;`
  - `grant all privileges on <db_name>.* to '<pfeadv>'@'localhost';`
- mysql, update, user, acces, host
  - `UPDATE mysql.user SET Host='%' WHERE Host='localhost' AND User='username';`
  - `FLUSH PRIVILEGES;`
- macos, create, bootable, usb, disk, iso, burn
  - when the installer is not working, we can change the version and it works
  - `sudo plutil -replace CFBundleShortVersionString -string "12.6.03" /Applications/Install\ macOS\ Sierra.app/Contents/Info.plist`
  - [source](https://stackoverflow.com/a/64201813/5761952)

- spoof, location, firefox, devtool
  - about:config
  - geo.provider.network.url
  - data:application/json,{"location": {"lat": -31.969195, "lng": 115.884545}, "accuracy": 27000.0}
  - [source](https://security.stackexchange.com/questions/147166/how-can-you-fake-geolocation-in-firefox)
- macos, fork, dead, process, ansible-playbook
  - `export OBJC_DISABLE_INITIALIZE_FORK_SAFETY='YES'`
  - [explaination](https://stackoverflow.com/a/73738232/5761952)
- iterm, skhd, activate, terminal, shortcut
  - [source](https://apple.stackexchange.com/a/333082)



## Archlinux hell

- `urxvt-unicode` from community needs perl modules
  - `yay -S perl-pod-parser`

## root

- forensic, file, iso, image
  - `testdisk` used to analyse and repaire disk images
  - `exiftool` read and write meta information from various files
- grub, boot, root bypass
  - edit grub entry
  - instead of running `ro quiet` set to `rw init=/bin/bash`
  - in prompt now you can remount /
    - `mount -n -o remount,rw /`
    - `passwd`


## Rand(websites)

- https://doesmysiteneedhttps.com/
- https://12factor.net/
- swap, file, create, ram,
  - https://aws.amazon.com/premiumsupport/knowledge-center/ec2-memory-swap-file/
- resize, partition, cloud, tool
  - https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/recognize-expanded-volume-linux.html
- oom, killer, linux, memory, segfault
  - https://unix.stackexchange.com/questions/136291/will-linux-start-killing-my-processes-without-asking-me-if-memory-gets-short/136294#136294
- agile, triangle, iron, mgmt, waterfall
  - [atlassian.com](https://www.atlassian.com/agile/agile-at-scale/agile-iron-triangle?utm_source=newsletter-email&utm_medium=email&utm_campaign=jira-insiders-newsletter_august-2020_EML-7386&jobid=104776148&subid=1522909647)
- software, ressources, coding, whitepaper, library
  - https://resources.sei.cmu.edu/library/
- hugo, cms, static, commit
  - https://forestry.io/
- bash, pitfalls, mistakes, error
  - [bash](https://mywiki.wooledge.org/BashPitfalls#for_f_in_.24.28ls_.2A.mp3.29)
- elastic, elk, observability
  - [observability](https://www.elastic.co/blog/observability-with-the-elastic-stack)
- schema on write, schema on read
  - [read/write](https://www.elastic.co/blog/schema-on-write-vs-schema-on-read)
- dns, propagation, verification, global
  - [dnsmap](https://dnsmap.io/)
- oneliner, command, shell, useful, tips, tricks
  - [here](https://linuxcommandlibrary.com/basic/oneliners.html)
- observability, system, htop, monitoring
  - [here](https://docs.monadical.com/s/system-monitoring-tools#Bonus-tools)
- aws, cloudFront, S3, serve, static, website, jekyll, hugo
  - [here](https://aws.amazon.com/premiumsupport/knowledge-center/cloudfront-https-requests-s3/)
- ssl, haproxy, configuration, generator
  - [here](https://ssl-config.mozilla.org/#server=haproxy)
- paste, by, wetransfer, presentation
  - [here](https://pasteapp.com/home)
- whiteboard, online, canvas
  - [here](https://miro.com/login/)
- golang, resources, tutorials
  - [here](https://golangresources.com/)
- minecraft, computercraft, file, watcher, cloud
  - [here](https://cloud-catcher.squiddev.cc/)
- linux, server, gaming, gameserver, easy, install, auto, setup
  - [here](https://linuxgsm.com/)
- docker, build, images, without, daemon, google, cloud
  - [kaniko](https://github.com/GoogleContainerTools/kaniko)
- docker, build, multistage, tutorial
  - [tuto](https://codefresh.io/docker-tutorial/node_docker_multistage/)
## Whitepapers and documents
- cheatsheet, vim, bash, cheat, sheet
  - [here](https://quickref.me/)
