# Comparing `tmp/djfabric-0.0.2.tar.gz` & `tmp/djfabric-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djfabric-0.0.2.tar", last modified: Mon Apr 10 06:28:41 2023, max compression
+gzip compressed data, was "djfabric-0.0.3.tar", last modified: Sat Jul 29 16:32:50 2023, max compression
```

## Comparing `djfabric-0.0.2.tar` & `djfabric-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-10 06:28:41.774933 djfabric-0.0.2/
--rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-08-08 06:51:05.000000 djfabric-0.0.2/LICENSE
--rw-rw-r--   0 dev       (1000) dev       (1000)      161 2021-08-08 06:51:05.000000 djfabric-0.0.2/MANIFEST.in
--rw-rw-r--   0 dev       (1000) dev       (1000)      296 2023-04-10 06:28:41.774933 djfabric-0.0.2/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      346 2023-03-31 16:19:28.000000 djfabric-0.0.2/README.md
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-10 06:28:41.774933 djfabric-0.0.2/djfabric/
--rw-rw-r--   0 dev       (1000) dev       (1000)        0 2023-04-10 06:28:10.000000 djfabric-0.0.2/djfabric/__init__.py
--rw-rw-r--   0 dev       (1000) dev       (1000)     7650 2023-04-10 06:28:10.000000 djfabric-0.0.2/djfabric/fab.py
-drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-04-10 06:28:41.774933 djfabric-0.0.2/djfabric.egg-info/
--rw-rw-r--   0 dev       (1000) dev       (1000)      296 2023-04-10 06:28:41.000000 djfabric-0.0.2/djfabric.egg-info/PKG-INFO
--rw-rw-r--   0 dev       (1000) dev       (1000)      261 2023-04-10 06:28:41.000000 djfabric-0.0.2/djfabric.egg-info/SOURCES.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-04-10 06:28:41.000000 djfabric-0.0.2/djfabric.egg-info/dependency_links.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       60 2023-04-10 06:28:41.000000 djfabric-0.0.2/djfabric.egg-info/requires.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)        9 2023-04-10 06:28:41.000000 djfabric-0.0.2/djfabric.egg-info/top_level.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       60 2023-04-10 05:02:33.000000 djfabric-0.0.2/requirements.txt
--rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-04-10 06:28:41.774933 djfabric-0.0.2/setup.cfg
--rw-rw-r--   0 dev       (1000) dev       (1000)      528 2023-04-10 05:04:36.000000 djfabric-0.0.2/setup.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-29 16:32:50.955711 djfabric-0.0.3/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      746 2021-08-08 06:51:05.000000 djfabric-0.0.3/LICENSE
+-rw-rw-r--   0 dev       (1000) dev       (1000)      161 2021-08-08 06:51:05.000000 djfabric-0.0.3/MANIFEST.in
+-rw-rw-r--   0 dev       (1000) dev       (1000)      296 2023-07-29 16:32:50.955711 djfabric-0.0.3/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      346 2023-03-31 16:19:28.000000 djfabric-0.0.3/README.md
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-29 16:32:50.955711 djfabric-0.0.3/djfabric/
+-rw-rw-r--   0 dev       (1000) dev       (1000)        0 2023-04-10 06:28:10.000000 djfabric-0.0.3/djfabric/__init__.py
+-rw-rw-r--   0 dev       (1000) dev       (1000)    10435 2023-07-29 16:08:34.000000 djfabric-0.0.3/djfabric/fab.py
+drwxrwxr-x   0 dev       (1000) dev       (1000)        0 2023-07-29 16:32:50.955711 djfabric-0.0.3/djfabric.egg-info/
+-rw-rw-r--   0 dev       (1000) dev       (1000)      296 2023-07-29 16:32:50.000000 djfabric-0.0.3/djfabric.egg-info/PKG-INFO
+-rw-rw-r--   0 dev       (1000) dev       (1000)      261 2023-07-29 16:32:50.000000 djfabric-0.0.3/djfabric.egg-info/SOURCES.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        1 2023-07-29 16:32:50.000000 djfabric-0.0.3/djfabric.egg-info/dependency_links.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       81 2023-07-29 16:32:50.000000 djfabric-0.0.3/djfabric.egg-info/requires.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)        9 2023-07-29 16:32:50.000000 djfabric-0.0.3/djfabric.egg-info/top_level.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       81 2023-07-29 15:21:52.000000 djfabric-0.0.3/requirements.txt
+-rw-rw-r--   0 dev       (1000) dev       (1000)       79 2023-07-29 16:32:50.955711 djfabric-0.0.3/setup.cfg
+-rw-rw-r--   0 dev       (1000) dev       (1000)      528 2023-07-29 16:32:25.000000 djfabric-0.0.3/setup.py
```

### Comparing `djfabric-0.0.2/LICENSE` & `djfabric-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `djfabric-0.0.2/djfabric/fab.py` & `djfabric-0.0.3/djfabric/fab.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,16 +15,19 @@
     'dump_db',
     'fetch_db',
     'fetch_media',
     'setup',
     'upload_env',
     'cert',
     'nginx_conf',
+    'restart_nginx',
     'supervisor_conf',
-    'unfold_to_server'
+    'unfold_to_server',
+    'upload_db',
+    'push_db',
 ]
 config = environ.Env()
 _STORAGE = {}
 
 
 @contextmanager
 def source():
@@ -91,14 +94,43 @@
         file_path
     ))
 
     run('rm {}'.format(file_path))
     local('rm {}'.format(file_path))
 
 
+def upload_db():
+    file_path = '/home/dev/{}_{}.sql'.format(
+        config('DB_NAME'),
+        datetime.now().strftime("%m-%d-%Y_%H-%M-%S")
+    )
+
+    local('pg_dump {} > {}'.format(config('DB_NAME'), file_path))
+
+    put(file_path, file_path)
+
+    return file_path
+
+
+def push_db():
+    file_path = upload_db()
+
+    run('sudo -u postgres psql -c "CREATE DATABASE {};"'.format(
+        config('DB_NAME')
+    ))
+
+    run('sudo -u postgres psql -d {} -f {}'.format(
+        config('DB_NAME'),
+        file_path
+    ))
+
+    run('rm {}'.format(file_path))
+    local('rm {}'.format(file_path))
+
+
 def setup():
     frame = sys._getframe()
     project_dir = dirname(frame.f_back.f_code.co_filename)
     config.read_env(join(project_dir, '.env'))
     env.project_dir = project_dir
     env.user = 'dev'
     env.hosts = [config('HOST')]
@@ -111,14 +143,16 @@
         '/home/dev/sites/{}/{}/.env'.format(
             config('DOMAIN'), config('PROJECT_NAME'))
     )
 
 
 def cert():
     sudo(f"sudo certbot certonly --webroot -d {config('DOMAIN')} -w /var/www/html")
+    sudo("sudo nginx -t")
+    restart_nginx()
 
 
 def _get_tmp_dir():
     tmp_dir = join(env.project_dir, 'tmp')
     os.makedirs(tmp_dir, exist_ok=True)
     return tmp_dir
 
@@ -191,23 +225,27 @@
     put(
         tmp_file_path,
         f"/etc/nginx/sites-available/{project_name}",
         use_sudo=True
     )
 
     sudo(f"sudo ln -s /etc/nginx/sites-available/{project_name} /etc/nginx/sites-enabled")
+    restart_nginx()
+
+
+def restart_nginx():
     sudo("sudo nginx -t")
     sudo("sudo systemctl restart nginx")
 
 
 def supervisor_conf():
     tmp_dir = _get_tmp_dir()
-    tmp_file_path = join(tmp_dir, config('PROJECT_NAME') + ".conf")
+    runsite_tmp_file_path = join(tmp_dir, config('PROJECT_NAME') + ".conf")
     _write_file(
-        tmp_file_path=tmp_file_path,
+        tmp_file_path=runsite_tmp_file_path,
         lines=[
             "[program:%(project_name)s]",
             "command=bash /home/dev/runsite.bash -d %(domain)s -n %(project_name)s -w 3 -s core.settings",
             "user=dev",
             "stdout_logfile=/home/dev/sites/%(domain)s/logs/supervisor.log",
             "autostart=True",
             "autorestart=true",
@@ -215,19 +253,71 @@
         ],
         params={
             "domain": config("DOMAIN"),
             "project_name": config('PROJECT_NAME'),
         }
     )
     put(
-        tmp_file_path,
+        runsite_tmp_file_path,
         "/etc/supervisor/conf.d",
         use_sudo=True
     )
 
+    if config('CELERY') == 'on':
+        celery_tmp_file_path = join(tmp_dir, config('PROJECT_NAME') + "-celery.conf")
+        _write_file(
+            tmp_file_path=celery_tmp_file_path,
+            lines=[
+                "[program:%(project_name)s_celery]",
+                "command=/home/dev/sites/%(domain)s/env/bin/celery -A core worker --loglevel=INFO --concurrency=10 %(worker)s --uid=1000",
+                "directory=/home/dev/sites/%(domain)s/%(project_name)s",
+                "autostart=true",
+                "autorestart=true",
+                "numprocs=1",
+                "stderr_logfile=/home/dev/sites/%(domain)s/logs/celery.err.log",
+                "stdout_logfile=/home/dev/sites/%(domain)s/logs/celery.out.log",
+                "startsecs=10",
+                "priority=1000"
+            ],
+            params={
+                "domain": config("DOMAIN"),
+                "project_name": config('PROJECT_NAME'),
+                "worker": "-n worker1.%%h"
+            }
+        )
+        put(
+            celery_tmp_file_path,
+            "/etc/supervisor/conf.d",
+            use_sudo=True
+        )
+
+        celery_beat_tmp_file_path = join(tmp_dir, config('PROJECT_NAME') + "-celery-beat.conf")
+        _write_file(
+            tmp_file_path=celery_beat_tmp_file_path,
+            lines=[
+                "[program:%(project_name)s_celery_beat]",
+                "command=/home/dev/sites/%(domain)s/env/bin/celery -A core beat --max-interval=7200 --loglevel=INFO",
+                "directory=/home/dev/sites/%(domain)s/%(project_name)s",
+                "autostart=true",
+                "autorestart=true",
+                "numprocs=1",
+                "startsecs=10",
+                "priority=1000"
+            ],
+            params={
+                "domain": config("DOMAIN"),
+                "project_name": config('PROJECT_NAME'),
+            }
+        )
+        put(
+            celery_beat_tmp_file_path,
+            "/etc/supervisor/conf.d",
+            use_sudo=True
+        )
+
     sudo("sudo supervisorctl reread")
     sudo("sudo supervisorctl update")
 
 
 def unfold_to_server():
     site_dir = f"/home/dev/sites/{config('DOMAIN')}"
     run(f"mkdir -p {join(site_dir, 'public', 'static')}")
@@ -239,14 +329,15 @@
 
     run(f"virtualenv {join(site_dir, 'env')} --python=/usr/bin/python3.8")
     run(f"ln -s {join(site_dir, 'env', 'bin', 'activate')} /home/dev/{config('PROJECT_NAME')}env")
     run(f"ln -s {join(site_dir, config('PROJECT_NAME'))} {config('PROJECT_NAME')}")
 
     upload_env()
     supervisor_conf()
+    cert()
     nginx_conf()
 
 
 def fetch_media():
 
     local_media_dir = join(env.project_dir, 'media')
     local('rm -r -f ' + local_media_dir)
```

### Comparing `djfabric-0.0.2/setup.py` & `djfabric-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 
 with open('requirements.txt') as f:
     requires = f.read().splitlines()
 
 
-version = '0.0.2'
+version = '0.0.3'
 url = 'https://github.com/pmaigutyak/djfabric'
 
 
 setup(
     name='djfabric',
     version=version,
     description='Django deploy app',
```

