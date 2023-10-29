Windows PowerShell
Copyright (C) Microsoft Corporation. All rights reserved.

Install the latest PowerShell for new features and improvements! https://aka.ms/PSWindows

PS C:\Users\Gozel> docker --help

Usage:  docker [OPTIONS] COMMAND

A self-sufficient runtime for containers

Common Commands:
  run         Create and run a new container from an image
  exec        Execute a command in a running container
  ps          List containers
  build       Build an image from a Dockerfile
  pull        Download an image from a registry
  push        Upload an image to a registry
  images      List images
  login       Log in to a registry
  logout      Log out from a registry
  search      Search Docker Hub for images
  version     Show the Docker version information
  info        Display system-wide information

Management Commands:
  builder     Manage builds
  buildx*     Docker Buildx (Docker Inc., v0.11.2-desktop.5)
  compose*    Docker Compose (Docker Inc., v2.23.0-desktop.1)
  container   Manage containers
  context     Manage contexts
  dev*        Docker Dev Environments (Docker Inc., v0.1.0)
  extension*  Manages Docker extensions (Docker Inc., v0.2.20)
  image       Manage images
  init*       Creates Docker-related starter files for your project (Docker Inc., v0.1.0-beta.9)
  manifest    Manage Docker image manifests and manifest lists
  network     Manage networks
  plugin      Manage plugins
  sbom*       View the packaged-based Software Bill Of Materials (SBOM) for an image (Anchore Inc., 0.6.0)
  scan*       Docker Scan (Docker Inc., v0.26.0)
  scout*      Docker Scout (Docker Inc., v1.0.9)
  system      Manage Docker
  trust       Manage trust on Docker images
  volume      Manage volumes

Swarm Commands:
  swarm       Manage Swarm

Commands:
  attach      Attach local standard input, output, and error streams to a running container
  commit      Create a new image from a container's changes
  cp          Copy files/folders between a container and the local filesystem
  create      Create a new container
  diff        Inspect changes to files or directories on a container's filesystem
  events      Get real time events from the server
  export      Export a container's filesystem as a tar archive
  history     Show the history of an image
  import      Import the contents from a tarball to create a filesystem image
  inspect     Return low-level information on Docker objects
  kill        Kill one or more running containers
  load        Load an image from a tar archive or STDIN
  logs        Fetch the logs of a container
  pause       Pause all processes within one or more containers
  port        List port mappings or a specific mapping for the container
  rename      Rename a container
  restart     Restart one or more containers
  rm          Remove one or more containers
  rmi         Remove one or more images
  save        Save one or more images to a tar archive (streamed to STDOUT by default)
  start       Start one or more stopped containers
  stats       Display a live stream of container(s) resource usage statistics
  stop        Stop one or more running containers
  tag         Create a tag TARGET_IMAGE that refers to SOURCE_IMAGE
  top         Display the running processes of a container
  unpause     Unpause all processes within one or more containers
  update      Update configuration of one or more containers
  wait        Block until one or more containers stop, then print their exit codes

Global Options:
      --config string      Location of client config files (default
                           "C:\\Users\\Gozel\\.docker")
  -c, --context string     Name of the context to use to connect to the
                           daemon (overrides DOCKER_HOST env var and
                           default context set with "docker context use")
  -D, --debug              Enable debug mode
  -H, --host list          Daemon socket to connect to
  -l, --log-level string   Set the logging level ("debug", "info",
                           "warn", "error", "fatal") (default "info")
      --tls                Use TLS; implied by --tlsverify
      --tlscacert string   Trust certs signed only by this CA (default
                           "C:\\Users\\Gozel\\.docker\\ca.pem")
      --tlscert string     Path to TLS certificate file (default
                           "C:\\Users\\Gozel\\.docker\\cert.pem")
      --tlskey string      Path to TLS key file (default
                           "C:\\Users\\Gozel\\.docker\\key.pem")
      --tlsverify          Use TLS and verify the remote
  -v, --version            Print version information and quit

Run 'docker COMMAND --help' for more information on a command.

For more help on how to use Docker, head to https://docs.docker.com/go/guides/
PS C:\Users\Gozel> docker desktop
docker: 'desktop' is not a docker command.
See 'docker --help'
PS C:\Users\Gozel> docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
docker: invalid reference format: repository name must be lowercase.
See 'docker run --help'.
PS C:\Users\Gozel> docker run --help

Usage:  docker run [OPTIONS] IMAGE [COMMAND] [ARG...]

Create and run a new container from an image

Aliases:
  docker container run, docker run

Options:
      --add-host list                  Add a custom host-to-IP mapping
                                       (host:ip)
      --annotation map                 Add an annotation to the container
                                       (passed through to the OCI
                                       runtime) (default map[])
  -a, --attach list                    Attach to STDIN, STDOUT or STDERR
      --blkio-weight uint16            Block IO (relative weight),
                                       between 10 and 1000, or 0 to
                                       disable (default 0)
      --blkio-weight-device list       Block IO weight (relative device
                                       weight) (default [])
      --cap-add list                   Add Linux capabilities
      --cap-drop list                  Drop Linux capabilities
      --cgroup-parent string           Optional parent cgroup for the
                                       container
      --cgroupns string                Cgroup namespace to use
                                       (host|private)
                                       'host':    Run the container in
                                       the Docker host's cgroup namespace
                                       'private': Run the container in
                                       its own private cgroup namespace
                                       '':        Use the cgroup
                                       namespace as configured by the
                                                  default-cgroupns-mode
                                       option on the daemon (default)
      --cidfile string                 Write the container ID to the file
      --cpu-period int                 Limit CPU CFS (Completely Fair
                                       Scheduler) period
      --cpu-quota int                  Limit CPU CFS (Completely Fair
                                       Scheduler) quota
      --cpu-rt-period int              Limit CPU real-time period in
                                       microseconds
      --cpu-rt-runtime int             Limit CPU real-time runtime in
                                       microseconds
  -c, --cpu-shares int                 CPU shares (relative weight)
      --cpus decimal                   Number of CPUs
      --cpuset-cpus string             CPUs in which to allow execution
                                       (0-3, 0,1)
      --cpuset-mems string             MEMs in which to allow execution
                                       (0-3, 0,1)
  -d, --detach                         Run container in background and
                                       print container ID
      --detach-keys string             Override the key sequence for
                                       detaching a container
      --device list                    Add a host device to the container
      --device-cgroup-rule list        Add a rule to the cgroup allowed
                                       devices list
      --device-read-bps list           Limit read rate (bytes per second)
                                       from a device (default [])
      --device-read-iops list          Limit read rate (IO per second)
                                       from a device (default [])
      --device-write-bps list          Limit write rate (bytes per
                                       second) to a device (default [])
      --device-write-iops list         Limit write rate (IO per second)
                                       to a device (default [])
      --disable-content-trust          Skip image verification (default true)
      --dns list                       Set custom DNS servers
      --dns-option list                Set DNS options
      --dns-search list                Set custom DNS search domains
      --domainname string              Container NIS domain name
      --entrypoint string              Overwrite the default ENTRYPOINT
                                       of the image
  -e, --env list                       Set environment variables
      --env-file list                  Read in a file of environment variables
      --expose list                    Expose a port or a range of ports
      --gpus gpu-request               GPU devices to add to the
                                       container ('all' to pass all GPUs)
      --group-add list                 Add additional groups to join
      --health-cmd string              Command to run to check health
      --health-interval duration       Time between running the check
                                       (ms|s|m|h) (default 0s)
      --health-retries int             Consecutive failures needed to
                                       report unhealthy
      --health-start-period duration   Start period for the container to
                                       initialize before starting
                                       health-retries countdown
                                       (ms|s|m|h) (default 0s)
      --health-timeout duration        Maximum time to allow one check to
                                       run (ms|s|m|h) (default 0s)
      --help                           Print usage
  -h, --hostname string                Container host name
      --init                           Run an init inside the container
                                       that forwards signals and reaps
                                       processes
  -i, --interactive                    Keep STDIN open even if not attached
      --ip string                      IPv4 address (e.g., 172.30.100.104)
      --ip6 string                     IPv6 address (e.g., 2001:db8::33)
      --ipc string                     IPC mode to use
      --isolation string               Container isolation technology
      --kernel-memory bytes            Kernel memory limit
  -l, --label list                     Set meta data on a container
      --label-file list                Read in a line delimited file of labels
      --link list                      Add link to another container
      --link-local-ip list             Container IPv4/IPv6 link-local
                                       addresses
      --log-driver string              Logging driver for the container
      --log-opt list                   Log driver options
      --mac-address string             Container MAC address (e.g.,
                                       92:d0:c6:0a:29:33)
  -m, --memory bytes                   Memory limit
      --memory-reservation bytes       Memory soft limit
      --memory-swap bytes              Swap limit equal to memory plus
                                       swap: '-1' to enable unlimited swap
      --memory-swappiness int          Tune container memory swappiness
                                       (0 to 100) (default -1)
      --mount mount                    Attach a filesystem mount to the
                                       container
      --name string                    Assign a name to the container
      --network network                Connect a container to a network
      --network-alias list             Add network-scoped alias for the
                                       container
      --no-healthcheck                 Disable any container-specified
                                       HEALTHCHECK
      --oom-kill-disable               Disable OOM Killer
      --oom-score-adj int              Tune host's OOM preferences (-1000
                                       to 1000)
      --pid string                     PID namespace to use
      --pids-limit int                 Tune container pids limit (set -1
                                       for unlimited)
      --platform string                Set platform if server is
                                       multi-platform capable
      --privileged                     Give extended privileges to this
                                       container
  -p, --publish list                   Publish a container's port(s) to
                                       the host
  -P, --publish-all                    Publish all exposed ports to
                                       random ports
      --pull string                    Pull image before running
                                       ("always", "missing", "never")
                                       (default "missing")
  -q, --quiet                          Suppress the pull output
      --read-only                      Mount the container's root
                                       filesystem as read only
      --restart string                 Restart policy to apply when a
                                       container exits (default "no")
      --rm                             Automatically remove the container
                                       when it exits
      --runtime string                 Runtime to use for this container
      --security-opt list              Security Options
      --shm-size bytes                 Size of /dev/shm
      --sig-proxy                      Proxy received signals to the
                                       process (default true)
      --stop-signal string             Signal to stop the container
      --stop-timeout int               Timeout (in seconds) to stop a
                                       container
      --storage-opt list               Storage driver options for the
                                       container
      --sysctl map                     Sysctl options (default map[])
      --tmpfs list                     Mount a tmpfs directory
  -t, --tty                            Allocate a pseudo-TTY
      --ulimit ulimit                  Ulimit options (default [])
  -u, --user string                    Username or UID (format:
                                       <name|uid>[:<group|gid>])
      --userns string                  User namespace to use
      --uts string                     UTS namespace to use
  -v, --volume list                    Bind mount a volume
      --volume-driver string           Optional volume driver for the
                                       container
      --volumes-from list              Mount volumes from the specified
                                       container(s)
  -w, --workdir string                 Working directory inside the container
PS C:\Users\Gozel> docker pull postgres
Using default tag: latest
latest: Pulling from library/postgres
a378f10b3218: Pull complete
2ebc5690e391: Pull complete
8fe57f734687: Pull complete
a2ddbb09cd9a: Pull complete
5a2499e87ab8: Pull complete
a45f5c4adf1b: Pull complete
178017fd978e: Pull complete
428dff1cb77d: Pull complete
4667364adfc4: Pull complete
4eea1f5281a9: Pull complete
369467411787: Pull complete
51184495a2bc: Pull complete
d3e246f01410: Pull complete
Digest: sha256:3d9ed832906091d609cfd6f283e79492ace01ba15866b21d8a262e8fd1cdfb55
Status: Downloaded newer image for postgres:latest
docker.io/library/postgres:latest

What's Next?
  View a summary of image vulnerabilities and recommendations → docker scout quickview postgres
PS C:\Users\Gozel> docker run -d --name container -p 5432:5432 -e POSTGRES_PASSWORD=dist_pass_123 postgres
25645b4fcf7ac0611d26fd9b9b234d995d1ddd60828393dda5ac82e53e34c47b
PS C:\Users\Gozel> docker [s
docker: '[s' is not a docker command.
See 'docker --help'
PS C:\Users\Gozel> docker ps
CONTAINER ID   IMAGE      COMMAND                  CREATED          STATUS          PORTS                    NAMES
25645b4fcf7a   postgres   "docker-entrypoint.s…"   18 seconds ago   Up 18 seconds   0.0.0.0:5432->5432/tcp   container
PS C:\Users\Gozel> docker exec -it container bash
root@25645b4fcf7a:/# psql -h localhost -U postgres
psql (16.0 (Debian 16.0-1.pgdg120+1))
Type "help" for help.

postgres=# create database gozel;
CREATE DATABASE
postgres=# \l
                                                      List of databases
   Name    |  Owner   | Encoding | Locale Provider |  Collate   |   Ctype    | ICU Locale | ICU Rules |   Access privileges
-----------+----------+----------+-----------------+------------+------------+------------+-----------+-----------------------
 gozel     | postgres | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           |
 postgres  | postgres | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           |
 template0 | postgres | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           | =c/postgres          +
           |          |          |                 |            |            |            |           | postgres=CTc/postgres
 template1 | postgres | UTF8     | libc            | en_US.utf8 | en_US.utf8 |            |           | =c/postgres          +
           |          |          |                 |            |            |            |           | postgres=CTc/postgres
(4 rows)

postgres=# \c gozel
You are now connected to database "gozel" as user "postgres".
gozel=# create table ASYNC_MESSAGES (

 RECORD_ID auto increment number,

 SENDER_NAME varchar(30),

 MESSAGE varchar(30),

 SENT_TIME DATE/TIME,

 RECEIVED_TIME DATA/TIME)

gozel-# ;
ERROR:  syntax error at or near "increment"
LINE 3:  RECORD_ID auto increment number,
                        ^
gozel=# CREATE TABLE ASYNC_MESSAGES (
    RECORD_ID SERIAL PRIMARY KEY, -- Auto-incremented number
    SENDER_NAME VARCHAR(30),
    MESSAGE VARCHAR(30),
    SENT_TIME TIMESTAMPTZ, -- Storing date and time with timezone information
    RECEIVED_TIME TIMESTAMPTZ -- Storing date and time with timezone information
);
CREATE TABLE
gozel=# \ds
                      List of relations
 Schema |             Name             |   Type   |  Owner
--------+------------------------------+----------+----------
 public | async_messages_record_id_seq | sequence | postgres
(1 row)

gozel=# \dt
             List of relations
 Schema |      Name      | Type  |  Owner
--------+----------------+-------+----------
 public | async_messages | table | postgres
(1 row)

gozel=# CREATE USER dist_user WITH PASSWORD 'dist_pass_123';
GRANT ALL PRIVILEGES ON TABLE ASYNC_MESSAGES TO dist_user;
CREATE ROLE
GRANT
gozel=# ALTER USER dist_user CONNECTION LIMIT -1;
ALTER USER dist_user VALID UNTIL 'infinity';
ALTER ROLE
ALTER ROLE
gozel=# exit
root@25645b4fcf7a:/# exit
exit
PS C:\Users\Gozel> docker ps
CONTAINER ID   IMAGE      COMMAND                  CREATED          STATUS          PORTS                    NAMES
25645b4fcf7a   postgres   "docker-entrypoint.s…"   55 minutes ago   Up 55 minutes   0.0.0.0:5432->5432/tcp   container
PS C:\Users\Gozel> docker exec -it container bash
root@25645b4fcf7a:/# ls
bin   dev                         etc   lib    lib64   media  opt   root  sbin  sys  usr
boot  docker-entrypoint-initdb.d  home  lib32  libx32  mnt    proc  run   srv   tmp  var
root@25645b4fcf7a:/# cd etc
root@25645b4fcf7a:/etc# ls
adduser.conf            dpkg          host.conf     libaudit.conf  nsswitch.conf      profile.d    rmt       subuid
alternatives            e2scrub.conf  hostname      locale.alias   opt                protocols    rpc       systemd
apt                     environment   hosts         locale.gen     os-release         rc0.d        security  terminfo
bash.bashrc             ethertypes    init.d        localtime      pam.conf           rc1.d        selinux   timezone
bindresvport.blacklist  fstab         inputrc       logcheck       pam.d              rc2.d        services  ucf.conf
cron.d                  gai.conf      issue         login.defs     passwd             rc3.d        shadow    update-motd.d
cron.daily              group         issue.net     logrotate.d    passwd-            rc4.d        shadow-   X11
debconf.conf            group-        kernel        mke2fs.conf    perl               rc5.d        shells    xattr.conf
debian_version          gshadow       ld.so.cache   motd           postgresql         rc6.d        skel
default                 gshadow-      ld.so.conf    mtab           postgresql-common  rcS.d        ssl
deluser.conf            gss           ld.so.conf.d  networks       profile            resolv.conf  subgid
root@25645b4fcf7a:/etc# cd postgresql
root@25645b4fcf7a:/etc/postgresql# ls
root@25645b4fcf7a:/etc/postgresql# find pg_hba.conf
find: ‘pg_hba.conf’: No such file or directory
root@25645b4fcf7a:/etc/postgresql# cd ..
root@25645b4fcf7a:/etc# cd
root@25645b4fcf7a:~# find pg_hba.conf
find: ‘pg_hba.conf’: No such file or directory
root@25645b4fcf7a:~# cd /var/lib/pqsql
bash: cd: /var/lib/pqsql: No such file or directory
root@25645b4fcf7a:~# cd /var/lib/pgsql
bash: cd: /var/lib/pgsql: No such file or directory
root@25645b4fcf7a:~# cd /var/lib/
root@25645b4fcf7a:/var/lib# ls
apt  dpkg  misc  pam  postgresql  shells.state  systemd  ucf
root@25645b4fcf7a:/var/lib# cd p
pam/        postgresql/
root@25645b4fcf7a:/var/lib# cd postgresql/
root@25645b4fcf7a:/var/lib/postgresql# ls
data
root@25645b4fcf7a:/var/lib/postgresql# cd data/
root@25645b4fcf7a:/var/lib/postgresql/data# ls
base          pg_dynshmem    pg_logical    pg_replslot   pg_stat      pg_tblspc    pg_wal                postgresql.conf
global        pg_hba.conf    pg_multixact  pg_serial     pg_stat_tmp  pg_twophase  pg_xact               postmaster.opts
pg_commit_ts  pg_ident.conf  pg_notify     pg_snapshots  pg_subtrans  PG_VERSION   postgresql.auto.conf  postmaster.pid
root@25645b4fcf7a:/var/lib/postgresql/data# vi pg_hba.conf
bash: vi: command not found
root@25645b4fcf7a:/var/lib/postgresql/data# cat pg_hba.conf
# PostgreSQL Client Authentication Configuration File
# ===================================================
#
# Refer to the "Client Authentication" section in the PostgreSQL
# documentation for a complete description of this file.  A short
# synopsis follows.
#
# ----------------------
# Authentication Records
# ----------------------
#
# This file controls: which hosts are allowed to connect, how clients
# are authenticated, which PostgreSQL user names they can use, which
# databases they can access.  Records take one of these forms:
#
# local         DATABASE  USER  METHOD  [OPTIONS]
# host          DATABASE  USER  ADDRESS  METHOD  [OPTIONS]
# hostssl       DATABASE  USER  ADDRESS  METHOD  [OPTIONS]
# hostnossl     DATABASE  USER  ADDRESS  METHOD  [OPTIONS]
# hostgssenc    DATABASE  USER  ADDRESS  METHOD  [OPTIONS]
# hostnogssenc  DATABASE  USER  ADDRESS  METHOD  [OPTIONS]
#
# (The uppercase items must be replaced by actual values.)
#
# The first field is the connection type:
# - "local" is a Unix-domain socket
# - "host" is a TCP/IP socket (encrypted or not)
# - "hostssl" is a TCP/IP socket that is SSL-encrypted
# - "hostnossl" is a TCP/IP socket that is not SSL-encrypted
# - "hostgssenc" is a TCP/IP socket that is GSSAPI-encrypted
# - "hostnogssenc" is a TCP/IP socket that is not GSSAPI-encrypted
#
# DATABASE can be "all", "sameuser", "samerole", "replication", a
# database name, a regular expression (if it starts with a slash (/))
# or a comma-separated list thereof.  The "all" keyword does not match
# "replication".  Access to replication must be enabled in a separate
# record (see example below).
#
# USER can be "all", a user name, a group name prefixed with "+", a
# regular expression (if it starts with a slash (/)) or a comma-separated
# list thereof.  In both the DATABASE and USER fields you can also write
# a file name prefixed with "@" to include names from a separate file.
#
# ADDRESS specifies the set of hosts the record matches.  It can be a
# host name, or it is made up of an IP address and a CIDR mask that is
# an integer (between 0 and 32 (IPv4) or 128 (IPv6) inclusive) that
# specifies the number of significant bits in the mask.  A host name
# that starts with a dot (.) matches a suffix of the actual host name.
# Alternatively, you can write an IP address and netmask in separate
# columns to specify the set of hosts.  Instead of a CIDR-address, you
# can write "samehost" to match any of the server's own IP addresses,
# or "samenet" to match any address in any subnet that the server is
# directly connected to.
#
# METHOD can be "trust", "reject", "md5", "password", "scram-sha-256",
# "gss", "sspi", "ident", "peer", "pam", "ldap", "radius" or "cert".
# Note that "password" sends passwords in clear text; "md5" or
# "scram-sha-256" are preferred since they send encrypted passwords.
#
# OPTIONS are a set of options for the authentication in the format
# NAME=VALUE.  The available options depend on the different
# authentication methods -- refer to the "Client Authentication"
# section in the documentation for a list of which options are
# available for which authentication methods.
#
# Database and user names containing spaces, commas, quotes and other
# special characters must be quoted.  Quoting one of the keywords
# "all", "sameuser", "samerole" or "replication" makes the name lose
# its special character, and just match a database or username with
# that name.
#
# ---------------
# Include Records
# ---------------
#
# This file allows the inclusion of external files or directories holding
# more records, using the following keywords:
#
# include           FILE
# include_if_exists FILE
# include_dir       DIRECTORY
#
# FILE is the file name to include, and DIR is the directory name containing
# the file(s) to include.  Any file in a directory will be loaded if suffixed
# with ".conf".  The files of a directory are ordered by name.
# include_if_exists ignores missing files.  FILE and DIRECTORY can be
# specified as a relative or an absolute path, and can be double-quoted if
# they contain spaces.
#
# -------------
# Miscellaneous
# -------------
#
# This file is read on server startup and when the server receives a
# SIGHUP signal.  If you edit the file on a running system, you have to
# SIGHUP the server for the changes to take effect, run "pg_ctl reload",
# or execute "SELECT pg_reload_conf()".
#
# ----------------------------------
# Put your actual configuration here
# ----------------------------------
#
# If you want to allow non-local connections, you need to add more
# "host" records.  In that case you will also need to make PostgreSQL
# listen on a non-local interface via the listen_addresses
# configuration parameter, or via the -i or -h command line switches.

# CAUTION: Configuring the system for local "trust" authentication
# allows any local user to connect as any PostgreSQL user, including
# the database superuser.  If you do not trust all your local users,
# use another authentication method.


# TYPE  DATABASE        USER            ADDRESS                 METHOD

# "local" is for Unix domain socket connections only
local   all             all                                     trust
# IPv4 local connections:
host    all             all             127.0.0.1/32            trust
# IPv6 local connections:
host    all             all             ::1/128                 trust
# Allow replication connections from localhost, by a user with the
# replication privilege.
local   replication     all                                     trust
host    replication     all             127.0.0.1/32            trust
host    replication     all             ::1/128                 trust

host all all all scram-sha-256
root@25645b4fcf7a:/var/lib/postgresql/data# service posgresql restart
posgresql: unrecognized service
root@25645b4fcf7a:/var/lib/postgresql/data# service postgresql restart
No PostgreSQL clusters exist; see "man pg_createcluster" ... (warning).
root@25645b4fcf7a:/var/lib/postgresql/data# exit
exit
PS C:\Users\Gozel> docker restart container
container
PS C:\Users\Gozel> docker exec -it container bash
root@25645b4fcf7a:/# /etc/init.d/postgresql restart
No PostgreSQL clusters exist; see "man pg_createcluster" ... (warning).
root@25645b4fcf7a:/# /etc/init.d/postgresql restart
No PostgreSQL clusters exist; see "man pg_createcluster" ... (warning).
root@25645b4fcf7a:/#
PS C:\Users\Gozel>

I was unable to join to server from another computer remotely therefore I could only sent the operations. When my friend try to join the server it shows that there is no such user. 
