# Comparing `tmp/gitlabx-0.6.0-py3-none-any.whl.zip` & `tmp/gitlabx-0.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 12805 bytes, number of entries: 22
+Zip file size: 12992 bytes, number of entries: 22
 -rwxrwxrwx  2.0 unx        0 b- defN 23-Jun-28 23:28 gitlabx/__init__.py
 -rwxrwxrwx  2.0 unx      380 b- defN 23-Jun-29 10:14 gitlabx/abstract.py
 -rwxrwxrwx  2.0 unx     1611 b- defN 23-Jul-06 22:11 gitlabx/branches.py
--rwxrwxrwx  2.0 unx     2112 b- defN 23-Jul-08 11:59 gitlabx/commits.py
+-rwxrwxrwx  2.0 unx     2992 b- defN 23-Jul-09 15:28 gitlabx/commits.py
 -rwxrwxrwx  2.0 unx     1026 b- defN 23-Jun-29 11:24 gitlabx/deployments.py
 -rwxrwxrwx  2.0 unx      902 b- defN 23-Jun-29 11:24 gitlabx/events.py
 -rwxrwxrwx  2.0 unx     2795 b- defN 23-Jul-06 22:11 gitlabx/factories.py
 -rwxrwxrwx  2.0 unx      944 b- defN 23-Jun-29 11:24 gitlabx/issues.py
 -rwxrwxrwx  2.0 unx      984 b- defN 23-Jul-02 23:37 gitlabx/jobs.py
 -rwxrwxrwx  2.0 unx     1800 b- defN 23-Jul-07 01:09 gitlabx/member.py
 -rwxrwxrwx  2.0 unx     1204 b- defN 23-Jul-02 23:01 gitlabx/merge_request.py
 -rwxrwxrwx  2.0 unx     1233 b- defN 23-Jul-02 23:49 gitlabx/pipelines.py
 -rwxrwxrwx  2.0 unx     1121 b- defN 23-Jul-02 23:38 gitlabx/pipelines_schedules.py
 -rwxrwxrwx  2.0 unx      785 b- defN 23-Jun-29 11:24 gitlabx/project.py
 -rwxrwxrwx  2.0 unx      979 b- defN 23-Jun-29 11:24 gitlabx/projectLanguages.py
 -rwxrwxrwx  2.0 unx     1026 b- defN 23-Jun-29 11:24 gitlabx/repositories.py
--rwxrwxrwx  2.0 unx     2111 b- defN 23-Jul-08 14:49 gitlabx/repositoryTree.py
+-rwxrwxrwx  2.0 unx     2221 b- defN 23-Jul-24 15:16 gitlabx/repositoryTree.py
 -rwxrwxrwx  2.0 unx     1062 b- defN 23-Jul-02 23:34 gitlabx/trriggers.py
--rwxrwxrwx  2.0 unx     1675 b- defN 23-Jul-08 16:47 gitlabx-0.6.0.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-08 16:47 gitlabx-0.6.0.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jul-08 16:47 gitlabx-0.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1684 b- defN 23-Jul-08 16:47 gitlabx-0.6.0.dist-info/RECORD
-22 files, 25534 bytes uncompressed, 10115 bytes compressed:  60.4%
+-rwxrwxrwx  2.0 unx     1675 b- defN 23-Jul-29 17:00 gitlabx-0.6.1.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-29 17:00 gitlabx-0.6.1.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jul-29 17:00 gitlabx-0.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1684 b- defN 23-Jul-29 17:00 gitlabx-0.6.1.dist-info/RECORD
+22 files, 26524 bytes uncompressed, 10302 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: gitlabx/repositoryTree.py
 Comment: 
 
 Filename: gitlabx/trriggers.py
 Comment: 
 
-Filename: gitlabx-0.6.0.dist-info/METADATA
+Filename: gitlabx-0.6.1.dist-info/METADATA
 Comment: 
 
-Filename: gitlabx-0.6.0.dist-info/WHEEL
+Filename: gitlabx-0.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: gitlabx-0.6.0.dist-info/top_level.txt
+Filename: gitlabx-0.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: gitlabx-0.6.0.dist-info/RECORD
+Filename: gitlabx-0.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gitlabx/commits.py

```diff
@@ -5,44 +5,71 @@
 
 # Represents a software Project
 class Commits(AbstractGitLab):
 
 	def __init__(self,personal_access_token, gitlab_url = None):
 		super(Commits,self).__init__(personal_access_token=personal_access_token,gitlab_url=gitlab_url)
 	
-	def get_by_project(self, project_id):
+	def get_by_id(self, project_id, short_id):
+		commit = None
+		try:
+			logging.info("Start function: get details about one commit")
+			project = self.gl.projects.get(project_id)
+			commit = project.commits.get(short_id)
+			return commit.asdict()
+			
+		except Exception as e: 
+			logging.error("OS error: {0}".format(e))
+			logging.error(e.__dict__) 
+
+		logging.info("Retrieve get details about one commit")
+	
+	def get_by_project(self, project_id, details = False, diff = False):
 		
 		commit_list = []
 
 		try:
 			logging.info("Start function: get_commit_projeto")
 			project = self.gl.projects.get(project_id)
 
 			logging.info("Start function: get_Commits:"+project.name )
 			commits = project.commits.list(iterator=True,get_all=True)
 			project = project.asdict()
 			for	commit in commits:
 				commitX = commit.asdict()
 				commitX['project_id'] = project['id']
-				#commitX['merge_requests'] = commit.merge_requests()
-				#commitX['refs'] = commit.refs() 
-				#commitX['comments'] = commit.comments.list()
-				#commitX['statuses '] = commit.statuses.list()
+				if (details):
+					commitX['merge_requests'] = commit.merge_requests()
+					commitX['refs'] = commit.refs() 
+					
+					commitX['comments'] = self.__list(commit.comments.list(iterator=True,get_all=True))
+					commitX['statuses '] = self.__list(commit.statuses.list(iterator=True,get_all=True))
+					if (diff):
+						diffs = []
+						for diff_x in commit.diff(iterator=True,get_all=True): diffs.append(diff_x)
+						commitX['diff'] = diffs
+
 
 				commit_list.append(commitX)
 			
 		except Exception as e: 
 			logging.error("OS error: {0}".format(e))
 			logging.error(e.__dict__) 
 
 		logging.info("Retrieve All Project`s Commits")
 		
 		return commit_list
 	
-	
+	def __list (self, elements):
+		elements_list = []
+		for element in elements:
+			elements_list.append(element.asdict())
+		return elements_list
+
+
 	def get_all(self, today=False): 
 		
 		result = []
 		commit_list = []
 
 		try:
 			logging.info("Start function: get_Commits")
@@ -55,17 +82,18 @@
 				for	commit in commits:
 					commitX = commit.asdict()
 					commitX['project_id'] = project['id']
 					#commitX['merge_requests'] = commit.merge_requests()
 					#commitX['refs'] = commit.refs() 
 					#commitX['comments'] = commit.comments.list()
 					#commitX['statuses '] = commit.statuses.list()
-
+					
 					commit_list.append(commitX)
-			
+					break
+				break
 		except Exception as e: 
 			logging.error("OS error: {0}".format(e))
 			logging.error(e.__dict__) 
 
 		logging.info("Retrieve All Project Commits")
 		
 		return commit_list
```

## gitlabx/repositoryTree.py

```diff
@@ -10,31 +10,33 @@
 	
 	
 	def get_by_project(self, project_id):
 		
 		project_repository_tree = []
 
 		try:
-			logging.info("Start function: get_projects_repository_tree")
+			logging.info("Start function: get_project_repository_tree")
 			project = self.gl.projects.get(project_id)
 
-			logging.info("Start function: get_projects_repository_tree:"+project.name )
+			logging.info("Start function: get_project_repository_tree:"+project.name )
 			project_repository_tree_return = project.repository_tree(get_all=True, iterator=True)
 			
 			for item in project_repository_tree_return:
+				if item["type"] == 'blob':
+					file_info =  project.repository_blob(item["id"])
+					item["file_info"] = file_info
+						
 				item["project_id"] = project.id
-				project_repository_tree.append(item)
-
-				
+				project_repository_tree.append(item)				
 			
 		except Exception as e: 
 			logging.error("OS error: {0}".format(e))
 			logging.error(e.__dict__) 
 
-		logging.info("Retrieve All Project`s get_projects_repository_tree")
+		logging.info("Retrieve get_project_repository_tree")
 		
 		return project_repository_tree
 	
 	def get_all(self, today=False):
 		
 		projects = []
 		project_repository_tree = []
```

## Comparing `gitlabx-0.6.0.dist-info/METADATA` & `gitlabx-0.6.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabx
-Version: 0.6.0
+Version: 0.6.1
 Summary: Uma Lib para buscar dados do Gitlab
 Home-page: https://gitlab.com/immigrant-data-driven-development/libs/application/gitlab
 Author: Carlos Henrique Maulaz de Freitas
 Author-email: carlosmaulaz@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `gitlabx-0.6.0.dist-info/RECORD` & `gitlabx-0.6.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 gitlabx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gitlabx/abstract.py,sha256=mc5cmcD-klDfmHwo0HSl8itgsAiHx9nla1d5FQFjmcQ,380
 gitlabx/branches.py,sha256=f6Rx2o2WS_TLbS380_GZYhr6soOkHIjtHkVErXD7zRw,1611
-gitlabx/commits.py,sha256=zXscx-eiKvf4l9b8apFvPdfac5Z0-4tq3OT3fOu6gBM,2112
+gitlabx/commits.py,sha256=NAbs5HnShuOlpWON4Tb55OBCRvu1x0JNM-vbWQsucsA,2992
 gitlabx/deployments.py,sha256=sa8S9wmox-8ihRLwZq1mvpxKU5N8iKK0S7W8R1L11Q8,1026
 gitlabx/events.py,sha256=Nl6q0E3mc_x_XFlyGDNLj1m8Z5iieLiKfMs1HEvZTIY,902
 gitlabx/factories.py,sha256=KCiNkYpxBdOiZek2Xc99TZBt4ZuAYZnhQ1C9YL44w00,2795
 gitlabx/issues.py,sha256=WRiKt2Oz23quLD_8RoFCZfZwfxiYgRBs7N19DxFtDSw,944
 gitlabx/jobs.py,sha256=306PTUqAn9YjxRjy5Y7NOVcs75r79_JhMvJiqWvZMXE,984
 gitlabx/member.py,sha256=BmHjZJQ05WX-SMpEGTjV7U_Nk2HHyOxMudPVZ1Hiuvo,1800
 gitlabx/merge_request.py,sha256=CEM_mVTxh-mP7rwocPSpfcngZJAbGbnbTGAWGjgmw20,1204
 gitlabx/pipelines.py,sha256=P8QnCKI0E2T5__MJ-7rqXbpRm9Z4SBkJd-mKgytJOG0,1233
 gitlabx/pipelines_schedules.py,sha256=OYcWI7fn64WtHOZG7e5liQ8Vuv1osKiCq0eeDXAoaqo,1121
 gitlabx/project.py,sha256=28QdSWWM0swGkFC9LeCZW5mAXobXp02UKNZYEIhky50,785
 gitlabx/projectLanguages.py,sha256=qhRf543cotBVMdAlkaZ_CW9KU1y9e2Pxyw6Vsj4zkls,979
 gitlabx/repositories.py,sha256=o5p06Cf_x1hXmltKiecFvWO1MyQyX5L6jLy-He0_sgs,1026
-gitlabx/repositoryTree.py,sha256=vahEwCg-7oTKH5UafRNBIrt00-tZSr1qv7MkjaHQ8sA,2111
+gitlabx/repositoryTree.py,sha256=eWOKidMofFbqXe9_HTfAoVT3NTJh7PDwWdgoJQ4N3oA,2221
 gitlabx/trriggers.py,sha256=KanV0r_eERuTMhsK6d2ZRxzhzkQFwnyHE-_gfLbUNks,1062
-gitlabx-0.6.0.dist-info/METADATA,sha256=5Gqt1omVcJvTbOd-pG92174iB6AYW4yqQ2wNWL3Z1vg,1675
-gitlabx-0.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gitlabx-0.6.0.dist-info/top_level.txt,sha256=EkmcO7CZ14bNE_fgl8kFTFfgu1K7yvMO481rj0zu6ns,8
-gitlabx-0.6.0.dist-info/RECORD,,
+gitlabx-0.6.1.dist-info/METADATA,sha256=wsC_OzWLQeAPAJBiN5tHeH0VAYBe7ocipaoq7GbUNts,1675
+gitlabx-0.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gitlabx-0.6.1.dist-info/top_level.txt,sha256=EkmcO7CZ14bNE_fgl8kFTFfgu1K7yvMO481rj0zu6ns,8
+gitlabx-0.6.1.dist-info/RECORD,,
```

